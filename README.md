# //How to Display The all non repeated Charecter from a String...

// Print all non Repeated Charecter from a String :

import java.util.*;
import java.lang.*;
public class String1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
       Scanner sc = new Scanner(System.in);
       System.out.println("enter the String : ");
       String str = sc.nextLine();
       
       for(int i=0; i<str.length(); i++)
       {
    	   int count = 0;
    	   for(int j=0; j<str.length(); j++)
    	   {
    		   if(i==j) //checking with the same index value
    		   {
    			 continue;  
    		   }
    		   
    	       else
    		   { 
    	    	   if(str.charAt(i)==str.charAt(j)) // if the charecter matches then increase the count
    	    	   {
    			    count++;
    			    continue;
    	    	   }
    		   }
    		   
    	   }
    	   if(count==0)
    	   {
    		  char a = (char) str.charAt(i);
    		  System.out.print(a);
    	   }
       }
	}

}
