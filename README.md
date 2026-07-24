import java.util.Scanner;
public class hour {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int hour, min, addmin, rehour, remin;
        hour = input.nextInt();
        min = input.nextInt();
        addmin = input.nextInt();
        min += hour * 60; //แปลงhourทั้งหมดเป็นนาที
        rehour = ((min + addmin) / 60); //แปลงนาทีทั้งหมดเป็นชั่วโมง
        remin = (min + addmin) % 60; //นาทีที่เหลือจากrehour
        if (rehour > 24) {
            if (remin < 10)
                System.out.println("0" + rehour % 24 + ":0" + remin);
            else {
                System.out.println("0" + rehour % 24 + ":" + remin);
            }
        } else if (rehour >= 10 && rehour < 24) {
            if (remin < 10)
                System.out.println(rehour % 24 + ":0" + remin);
            else {
                System.out.println(rehour % 24 + ":" + remin);
            }
        } else if (rehour <= 1) {
            if (remin < 10)
                System.out.println("0" + rehour % 24 + ":0" + remin);
            else {
                System.out.println("0" + rehour % 24 + ":" + remin);
            }
        } else {
            if (remin < 10)
                System.out.println("0" + rehour % 24 + ":0" + remin);
            else {
                System.out.println("0" + rehour % 24 + ":" + remin);
            }
        }
    }
}
