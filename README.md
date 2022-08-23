import java.util.Scanner;

public class sr {
    public static void main(String[] args) {
        int kowshik[] = new int[1000];
        int i,j,swap;
        System.out.println("Enter the SIZE: ");
        Scanner km = new Scanner(System.in);
        int n = km.nextInt();
        System.out.printf("Enter %d element input :  ",n);
        for(i=0;i<n;i++ )
        {
            kowshik[i] = km.nextInt();
        }
        for(i=0;i<n;i++)
        {
            j=i;
            while (j>0 && kowshik[j-1] > kowshik[j])
            {
                swap = kowshik[j];
                kowshik[j] = kowshik[j-1];
                kowshik[j-1] = swap;
                j--;

            }
        }
        System.out.println("After the Sorting : ");

            for(i=0;i<n;i++)
            {
                System.out.println(kowshik[i]);
            }
        System.out.println("");



    }
}
