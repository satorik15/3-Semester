# 3-Semester
package ru.mirea.kvbo1.toryanik;
import java.lang.*;
import java.util.Scanner;
import java.util.Set;

public class Main {
    public static void main(String[] args)
    {
        Square kvadrat = new Square(5);
        //System.out.println(kvadrat); ////////////////////////////////// First task
        //System.out.println("area="+kvadrat.GetArea());
        /*int[] massive = new int[10];
        Scanner sc  = new Scanner(System.in);
        double counter=0.0;
        for(int i=0;i<10;i++)
        {
            massive[i]=sc.nextInt();
            counter+=massive[i];
        }
        System.out.println("totalSum="+(int)counter);
        System.out.println("average"+ counter / 10);
        for(int i=0; i<10;i++)
        {
            System.out.println(massive[i]);
        }*/

        /* Scanner input = new Scanner(System.in); ////////////Second task
        int[] userArray = new int[10];
        for(int ind = 0; ind < userArray.length; ++ind)
        {
            userArray[ind] = input.nextInt();
        }
        OutputArray(userArray);
        System.out.println("The min number is: " + ChoiceNumberInArray(userArray, "min"));
        System.out.println("The max number is: " + ChoiceNumberInArray(userArray, "max"));
        System.out.println("The sum number is: " + ChoiceNumberInArray(userArray, "sum"));
    }
    public static int ChoiceNumberInArray(int[] checkArray, String choice) {
        if(choice == "min")
        {
            int min = checkArray[0];
            for(int ind : checkArray) {
                if(min > ind) {
                    min = ind;
                }
            }
            return min;
        } else if(choice == "max"){
            int max = checkArray[0];
            for(int ind : checkArray) {
                if(max < ind) {
                    max = ind;
                }
            }
            return max;
        } else {
            int sum = 0;
            for(int ind : checkArray) {
                sum += ind;
            }
            return sum;
        }

    }
    public static void OutputArray(int[] userArray) {
        for(int ind = 0; ind < userArray.length; ++ind) {
            System.out.println(userArray[ind]);
        } */
    //////task 3\
        /*
        if (args.length > 1 && str1.equals(str2))
            System.out.println("OK");
        else
            System.out.println("KO");
        */
        /////task 4
        /*for(int i=1;i<11;i++)
        {
            System.out.println("1/"+i);
        }
        ///////task 5
        /*Scanner input = new Scanner(System.in);
        Factorial task5 = new Factorial(input.nextInt());
        System.out.println(task5.calculateFactorial());*/
    }
}




package ru.mirea.kvbo1.toryanik;

public class Factorial {
    private int number;
    private int sum = 1;

    public int getNumber() {
        return number;
    }

    public void setNumber(int number) {
        this.number = number;
    }
    public int calculateFactorial() {
        for(int ind = 1; ind <= number; ind++) {
            sum *= ind;
        }
        return sum;
    }
    public Factorial(int number) {
        this.number = number;
    }
}




package ru.mirea.kvbo1.toryanik;

public class Square
{
    private double side;

    public double getSide() {
        return side;
    }

    public void setSide(double side) {
        this.side = side;
    }

    public Square(double side) {
        this.side = side;
    }

    @Override
    public String toString() {
        return "Square{" +
                "side=" + side +
                '}';
    }
    public  double GetArea()
    {
        return side * side;

    }
}

