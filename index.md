/**
 * @(#)fibonacci.java
 *
 *
 * @author 
 * @version 1.00 2018/1/12
 */
import javax.swing.JOptionPane;

public class fibonacci {
        
    /**
     * Creates a new instance of <code>fibonacci</code>.
     */
    public fibonacci() {
    }
    public static void main(String[] args)
    {
    int num;
    num = Integer.parseInt(JOptionPane.showInputDialog("Enter a number with the range of 5 - 100:"));
     int f = 0;
        int g = 1;

        for(int i = 1; i <= num; i++)
        {
            f = f + g;
            g = f - g;
            if (f>num){
            	break;
            }
            System.out.print(f + " ");
            
        }

        System.out.println();
    }
}
