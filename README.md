// Classe Point
class Point {
    // Attributs
    private float abscisse;
    private float ordonnee;

    // Constructeur par défaut
    public Point() {}

    // Constructeur avec deux paramètres
    public Point(float abscisse, float ordonnee) {
        this.abscisse = abscisse;
        this.ordonnee = ordonnee;
    }

    // Méthode affiche
    public void affiche() {
        System.out.println("<" + abscisse + ", " + ordonnee + ">");
    }

    // Redéfinition de la méthode toString
    @Override
    public String toString() {
        return "<" + abscisse + ", " + ordonnee + ">";
    }
}

// Classe TestPoint
public class TestPoint {
    public static void main(String[] args) {
        // Création d'un objet instance de la classe Point
        Point point = new Point(2.5f, 3.2f);
        
        // Invocation de la méthode affiche
        point.affiche();

        // Affichage en utilisant la méthode toString
        System.out.println(point); // point un objet instance de la classe Point.
    }
}