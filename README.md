# Arrays-Ds
import java.util.*;
public class reverse{
    public static void main(String[] args)
    {
        int n,i,t;
        Scanner sc = new Scanner(System.in);
        n=sc.nextInt();
        int a[]=new int[n];
        for(i=0;i<n;i++){
            a[i]=sc.nextInt();
        }
        t=n-1;
        for(i=0;i<n/2;i++){
            int temp=a[i];
            a[i]=a[t];
            a[t]=temp;
            t--;

        }
        for(i=0;i<n;i++){
            System.out.print(a[i]+" ");
        }
    }
}
