# Enbuyuk_Enkucuk-bulma-dizi-olmadan
www.patika.dev Dizi olmadan en buyuk en kucuk bulma



        import java.util.Scanner;

        public class En_buyuk_en_kucuk {
        public static void main(String[] args) {
        int n;
        int min=1,max=1;
        int number;
        System.out.println("Kac sayi gireceksiniz?");
        Scanner input=new Scanner(System.in);
        n=input.nextInt();
        for (int i=1;i<=n;i++){
            System.out.println(i+". sayiyi giriniz:");
            number=input.nextInt();
            if(i==1){
                min=number;
                max=number;
            }
            if(number>max){
                max=number;
            }
            if(number<min){
                min=number;
            }
        }
            System.out.println("En buyuk: "+max);
            System.out.println("En kucuk: "+min);
    }
}
