# ProjectPrize
import java.util.Scanner;

public class P05_ProjectPrize {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        int partsOfProject = Integer.parseInt(scanner.nextLine());
        double moneyPrizePerPoint = Double.parseDouble(scanner.nextLine());
        int sumPoints = 0;
        int counter = 0;


        while(counter < partsOfProject){

            int currentProjectPoints = Integer.parseInt(scanner.nextLine());

            ++counter;

            if (counter % 2 == 0){
                currentProjectPoints = currentProjectPoints * 2;
            }

            sumPoints = sumPoints + currentProjectPoints;

        }

        double projectPrice = sumPoints * moneyPrizePerPoint;

        System.out.printf("The project prize was %.2f lv.", projectPrice );
    }

}
