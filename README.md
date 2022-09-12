# ebobEkok


import java.util.Scanner;
public class Main {


    public static void main(String[] args) {
    Scanner inp=new Scanner(System.in);
    int n1,n2;
    int ebob=1,ekok=1;
        System.out.println("Birinci Sayıyı Giriniz:");
        n1=inp.nextInt();
        System.out.println("Birinci Sayıyı Giriniz:");
        n2=inp.nextInt();
        int i=1,k=1;
        while (i <= n1) {
            if (n1 % i == 0 && n2 % i == 0) {
                //   System.out.print(i+" ");
                ebob = i;
            }
            i++;
        }
        System.out.println("EBOB:" + ebob);
        while (k <= (n1 * n2)) {
            if (k % n1 == 0 && k % n2 == 0) {
                ekok = k;
                break;
            }
            k++;
        }
        System.out.println("EKOK: " + ekok);

    }

}
