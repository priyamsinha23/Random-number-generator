# Random-number-generator

import java.util.Scanner;
import java.util.Random;

    public class Number_Guessing_Game {
        public static void main(String[] args) { 
            Scanner scanner = new Scanner(System.in);
            Random random = new Random() ;
            int min_Range = 1;
            int max_Range= 100 ;
            int generated_Number = random.nextInt(max_Range - min_Range + 1) + min_Range;
            System.out.println("Please choose a random number between " +min_Range + " to " +max_Range +".") ;
            
            int Guess_by_user; 
            do{
                System.out.print("Enter your guess ");
                Guess_by_user= scanner.nextInt() ; 
                
                 if( Guess_by_user >generated_Number){ 
         System.out.println("Too high");
        }
        else if( Guess_by_user < generated_Number){
        System.out.println("Too low");
        }
        else {
        System.out.println("You guessed the correct number.") ;
                
            }
        } while( Guess_by_user != generated_Number);
    }
    } 

        
