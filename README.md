import java.lang.reflect.Array;
import java.util.Arrays;

public class Lesson_1 {
    public static void main(String[] args) {
        int[] mass = create();
        System.out.println(Arrays.toString(mass));
        twoMass();
        checkSumSign();
        sameArray(4,5);
    }

    // 1
    static void printThreeWords() {
            System.out.println("Orange");
            System.out.println("Banana");
            System.out.println("Apple");
    }
    //2
    static void checkSumSign() {
        int num1 = 10;
        int num2 = 5;
        int num3 = num1 + num2;
        if (num3 >=0) {
            System.out.println("Сумма положительная");
        }else {
            System.out.println("Сумма отрицательная");
        }
    }
    //3
    static void printColor() {
        int value = 93;
        if (value < 0) {
            System.out.println("Красный");
        } else if (value >= 0 && value <= 100) {
            System.out.println("Желтый");
        } else  {
            System.out.println("Зеленый");
        }
    }
    //4
    static void compareNumbers() {
        int a = 15;
        int b = 10;
      if (a >= b) {
          System.out.println("a >= b");
      }else {
          System.out.println("a < b");
      }
    }
    //5
    static void sum(int a, int b) {
       int c = a + b;
       boolean x = (c >= 10) && (c <= 20);
        System.out.println(x);
    }
    //6
    static void number (int a){
        if (a >= 0) {
            System.out.println("Число положительное ");
        }else {
            System.out.println("Число отрицательное ");
        }
    }
    //7
    static void bool (int num) {
        boolean x = (num < 0);
        System.out.println(x);
    }
    //8
    static void printTime (int num) {
        for (int i = 0;i < num;i++) {
            System.out.println("printTime");
        }
    }
    //9
    static void year (int big) {
        boolean year = (big % 4 ==0 && big % 100 !=0) || (big % 400 ==0);
        System.out.println(year);
    }
    //10
    static void invert (int[] number) {
        for (int i = 0; i < number.length; i++) {
            if (number[i] == 0) {
                number[i] =1;
            }else {
                number[i] = 0;
            }
        }
    }
    //11
    static int[] create () {
        int[] mass = new int[100];
        for (int i = 0;i < mass.length;i++) {
            mass[i] = i + 1;
        }
        return mass;
    }
    //12
    static void six (int[] num) {
        for (int i = 0;i < num.length;i++) {
            if (num[i] < 6) {
                num[i] = i * 2;
            }
        }
    }
    //13
    static void twoMass () {
        int[][] more = new int[10][10];
        for (int i = 0;i < 10;i++){
            more[i][i] = 1;
        }
           for (int i = 0;i < 10;i++) {
               for (int l = 0;l < 10;l++) {
                   System.out.println(more[i][l] + "");
               }
           }
    }
    //14
    static void sameArray (int mas, int out) {
        int[] arr = new int[mas];
        for (int i = 0;i < mas;i++) {
            arr[i] = out;
            System.out.println(arr[i]);
        }
    }
}
