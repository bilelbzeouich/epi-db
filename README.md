import java.util.Scanner;

public class Couronne {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Demander à l'utilisateur d'entrer les rayons r1 et r2
        System.out.print("Entrez le rayon extérieur r1 : ");
        double r1 = scanner.nextDouble();
        
        System.out.print("Entrez le rayon intérieur r2 : ");
        double r2 = scanner.nextDouble();
        
        // Demander à l'utilisateur d'entrer les coordonnées du point P
        System.out.print("Entrez la coordonnée x du point P : ");
        double x = scanner.nextDouble();
        
        System.out.print("Entrez la coordonnée y du point P : ");
        double y = scanner.nextDouble();
        
        // Calculer la distance du point P à l'origine
        double distance = Math.sqrt(x*x + y*y);
        
        // Vérifier si le point se trouve à l'intérieur de la couronne
        if (distance >= r2 && distance <= r1) {
            System.out.println("Le point P se trouve à l'intérieur de la couronne.");
        } else {
            System.out.println("Le point P ne se trouve pas à l'intérieur de la couronne.");
        }
        
        scanner.close();
    }
}