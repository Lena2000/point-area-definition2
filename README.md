package var2;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class Var2 {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
      
            double c=5;
            double c1=20;
            double c2=35;
            double d=3;
            double d1=10;
            double d2=25; 
        System.out.println("Input your X: ");
        Scanner sc = new Scanner(System.in);
        int x = sc.nextInt();
        System.out.println("Input your Y: ");
        int y = sc.nextInt();
        if (x>c1 && x <c2 && y>0 && y<d2)
            System.out.println("Oblast B");
       //(x-c1)2 + (y-d1)2 = (d1-d)2
      else if (Math.pow((x-c1),2) + Math.pow((y-d1),2) <= Math.pow((d1-d),2) && y>d1 && x<c1)
       System.out.println("Oblast A");
      else System.out.println("Not any oblast");
    }
    
}
