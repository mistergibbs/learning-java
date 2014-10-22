/*
 * Array Assignment
 * 
 */

package gibbs_array_assignment;

import java.io.File;
import java.io.IOException;
import java.util.LinkedList;
import java.util.List;
import java.util.Scanner;


/**
 *
 * @author Brian Gibbs
 */

public class Gibbs_array_assignment  // begin class
{
    
    public static void main(String[] args) throws Exception // begin main
    {
     
String[] file = new String[100];
int count;
        
count = readEnroll(file);




count = readEnroll();
String[] enrollment = new String[count];



System.out.println("There are " + count + " sections for CIS 103");




     
     
     
     
   
    
            
    
    

    
    } // end main
    
    
    
    
    
    
 




/***************************************************************************
*
*                            Begin Methods
* 
/***************************************************************************/




 /****************************************************************
  * 
  * method - read data from array
  * 
 /****************************************************************/

public static int readEnroll(String[] lines) throws Exception       // this line creates a method that returns an integer value(the number of lines read), readEnroll and can be passed a string array 'lines'
{   
     int count = 0; // initialize array count

    // Create a File class object x and give it the name of the file to read
    java.io.File x = new java.io.File("enrollments.txt");

    
    
    // Create a Scanner named y to read the input stream from the file x
    Scanner y  = new Scanner(x);

    
    
    // Read a line of text from the file 
    while ( y.hasNextLine() )
    {
    lines[count] = y.nextLine();
    count ++; // increment count
    } // end while
    

    // print the message from the file on the screen
    System.out.println("reading from the data file...\n");
    System.out.println(enroll);
  
    // Close the input data strean and associated file
    y.close();  
    return count;
} // method
 /****************************************************************
  * 
  * end read data from array
  * 
 /****************************************************************/




        
 /****************************************************************
  * 
  * method - minimum value of array
  * 
 /****************************************************************/

public static double intMin(int arraylength)
{
int[] enroll = new int[arraylength]; 

int i = 0;
int minimum;
minimum = enroll[i];
for(i= 1; i < enroll.length(); i++); // iterate starting at the second element
if ( enroll[i] < minimum )
    minimum = enroll[i];
return minimum;  
}
 /****************************************************************
  * 
  * end minimum data of array
  * 
 /****************************************************************





 /****************************************************************
  * 
  * method - maximum value of array
  * 
 /****************************************************************/

public static double intMax(int arraylength) 
{
int[] enroll = new int[arraylength]; 
int i = 0;
int maximum;
maximum = enroll[i];
for( i= 1; i < enroll.length(); i++); // iterate starting at the second element
if ( enroll[i] >  maximum)
    maximum = enroll[i];
return maximum;
}
 /****************************************************************
  * 
  * end maximum value of array
  * 
 /****************************************************************
 




 /****************************************************************
  * 
  * method - average value of array objects
  * 
 /****************************************************************/

public static double intAverage(int arraylength) 
{
int[] numbers = new int[arraylength];


//calculate sum of all array elements

int sum = 0;

for(int i=0; i < numbers.length ; i++)
sum = sum + numbers[i];


//average equals sum divided bynumber of objects in array

double average = sum / numbers.length();

// return 'average' value to method
return average;
}
 /****************************************************************
  * 
  * end average value of array objects
  * 
 /****************************************************************/

} //end class
