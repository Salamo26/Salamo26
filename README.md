
import java.util.Random;

public class GamblingGame {
    public static void main(String[] args) {
        Random random = new Random();
        int userNumber = random.nextInt(10); // يمكنك تغيير الرقم 10 حسب احتياجاتك
        int guess = random.nextInt(10);
        
        System.out.println("الرقم المخفي هو: " + userNumber);
        System.out.println("حاول تخمين الرقم بين 0 و 9: " + guess);
        
        if (guess == userNumber) {
            System.out.println("تهانينا! لقد فزت باللعبة!");
        } else {
            System.out.println("آسف، لم تفز هذه المرة. حاول مرة أخرى!");
        }
    }
}
