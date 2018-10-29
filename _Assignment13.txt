
package assignment13;
import java.util.Scanner;

public class Assignment13 {

   
    public static void main(String[] args) {
        Scanner keyboard = new Scanner(System.in);
       int markCount;
       System.out.print("How many marks for this student ?");
       markCount = keyboard.nextInt();
       
       int[] marks = new int [markCount];     //creating of array
        int i,j;    
        float avg = 0;//lets loop
        for(i=0; i < markCount; i++){
            System.out.print("Please enter mark " + (i+1) + ":");
        marks[i] = keyboard.nextInt();
        
    }
        
     for(j=0; j< markCount;j++){
       avg = (avg + marks[j]);
         System.out.println("marks" + (j+1) + ":" +marks[j]);
     }
     System.out.println("The average is: " + (avg/markCount));
      
}}
