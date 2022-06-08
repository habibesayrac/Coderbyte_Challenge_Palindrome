# Coderbyte_Challenge_Palindrome

import java.util.*; 
import java.io.*;

class Main {

  public static String Palindrome(String str) {
       
    str = str.toLowerCase();

    String strNoSpace=str.replaceAll("\\s","");

         int length = strNoSpace.length();

    String strReverse ="";
   

    for(int i =length-1; i>=0; i--){


      strReverse = strReverse+ strNoSpace.charAt(i);

    }
   
    if(strReverse.equals(strNoSpace)){
      return "true";
    } else{
      return "false";
    }
  
  }

  public static void main (String[] args) {  
    // keep this function call here     
    Scanner s = new Scanner(System.in);
    System.out.print(Palindrome(s.nextLine())); 
  }

}
