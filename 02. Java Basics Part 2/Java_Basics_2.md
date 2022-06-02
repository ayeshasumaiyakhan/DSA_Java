## Java Basics 2 problems

> Try to Solve by your own and go to the solution only when you are stuck 

#### Problem 1: Java program to find the numbers greater than the avargae of the numbers of a given array

```java
import java.util.*;
public class Main {
  public static void main(String[] args) 
    {
      Integer nums[] = new Integer[]{1, 20, 13, 3, 25, 2, 15};
      int sum = 0;
	  System.out.println("Original Array: ");
	  System.out.println(Arrays.toString(nums));
	  for(int i = 0; i < nums.length; i++) {      
      sum = sum + nums[i];
    }
      double average = sum / nums.length;
      System.out.println("The average of the said array is: " + average);
      System.out.println("The numbers in the said array that are greater than the average are: ");
      for(int i = 0; i < nums.length; i++) {
      if(nums[i] > average) {
        System.out.println(nums[i]);
      }
    }
	}
}
```
>Output: <br>
>Original Array: <br>
>[1, 20, 13, 3, 25, 2, 15] <br>
>The average of the said array is: 11.0 <br>
>The numbers in the said array that are greater than the average are:  <br>
>20 <br>
>13 <br>
>25 <br>
>15 <br>

---------------------------------------------------------------------------------------------------------------

#### Problem 2: Write a Java program that takes a number as input and prints its muktiplication table upto 10.

```java
import java.util.*;
public class Main {
  public static void main(String[] args) 
    {
      Scanner sc = new Scanner(System.in);
      System.out.println("Enter the number to print the table:");
      int num = sc.nextInt();
      for(int i =1; i<=10;i++){
        System.out.println(num+"x"+i+"="+num*i);
        
      }

	}
}

```
>Output:
>Enter the number to print the table:<br>
> 3<br>
>3x1=3<br>
>3x2=6<br>
>3x3=9<br>
>3x4=12<br>
>3x5=15<br>
>3x6=18<br>
>3x7=21<br>
>3x8=24<br>
>3x9=27<br>
>3x10=30<br>

------------------------------------------------------------------------------

#### Problem 3: Write a java program to sum the values of an Array.
```java
import java.util.*;
public class Main {
  public static void main(String[] args) 
    {
      Integer nums[] = new Integer[]{1, 20, 13, 3, 25, 2, 15};
      int sum = 0;

      for(int i = 0; i < nums.length; i++) {      
        sum +=   nums[i];
      }
       System.out.println("The sum of the array is:"+ sum);
	}
}
```
> Output: <br>
> The sum of the array is:79 <br>
----------------------------------------------------------------------------------
#### Problem 4: Write a Java program to find the maximum and minimum value of an Array.

```java
import java.util.*;
public class Main {
  public static void main(String[] args) 
    {
      Integer nums[] = new Integer[]{1, 90, 0, 3, 25, 2, 0};
      int max = nums[0];
      int min = nums[0];

	  for(int i = 0; i < nums.length; i++) {      
      if(nums[i]<min){
        min =nums[i];
      }
      if(nums[i]>max){
        max =nums[i];
      }
    }
    System.out.println("Max Value:"+ max);
    System.out.println("Min Value:"+ min);
	}
}
```
> Output
> Max Value:90
> Min Value:0

-----------------------------------------------------------------------
Problem 5: Write a Java program to seperate 0s on the left side and 1s and on the right side
```java
import java.util.*;
public class Main {
  public static void main(String[] args) 
    {
      Integer nums[] = new Integer[]{1, 0, 0, 1, 1, 1, 0, 1, 1, 0};
      int count = 0;

	  for(int i = 0; i < nums.length; i++) {      
      if(nums[i] == 0){
        count++;
      }  }
    
    for(int i =0;i<count;i++){
      nums[i] = 0;
    }
    for(int i =count;i<nums.length;i++){
      nums[i] = 1;
    }
  for(int i =0;i<nums.length;i++){
    System.out.print(nums[i]+" ");
    }
 	}
}
```
>Output:
>0 0 0 0 1 1 1 1 1 1 

-----------------------------------------------------------------------
Problem 6: Write a java method to find the smallest among three numbers.
```java
import java.util.*;
public class Main {
  public static void main(String[] args) 
    {
      int a = 10;
      int b = 2;
      int c = 90;
      int min = 0;
      
      if(a < b && a<c){
          min =a;
      }else if(b<c &&b<a){
        min = b;
        
      }else{
        min = c;
      }
      System.out.println("Min: "+ min);
	}
}
```
>Output: 
>Min: 2

---------------------------------------------------------------------------------
Problem 7:Write a Java method to print Fibonacci series of n terms where n is argument passed by user.

> In fibonacci series, next number is the sum of previous two numbers for example 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55 etc. 

```java
import java.io.*;
import java.util.*;

class GFG {
	public static void main (String[] args) {
	int n1=0,n2=1,n3; 
     	Scanner sc = new Scanner(System.in);
    	 int N = sc.nextInt(); //10
     
    	 System.out.print(n1+" "+n2);//printing 0 and 1    
     	   
	for(int i=2;i<N;++i)//loop starts from 2 because 0 and 1 are already printed    
	{    
		n3=n1+n2;    
		System.out.print(" "+n3);    
		n1=n2;    
		n2=n3;    
	}    
	}
}
```
>Output: 
>0 1 1 2 3 5 8 13 21 34
--------------------------------------------------------------------------------------------------
Problem 8: Write a program to find the factorial value of any number entered through the keyboard.

```java
import java.io.*;

class GFG {
    public static void main (String[] args) {
	int i,fact=1;  
  	int number=5;//It is the number to calculate factorial    
  	for(i=1;i<=number;i++){    
          fact=fact*i;    
          }    
  System.out.println("Factorial of "+number+" is: "+fact);    	}
}

```
>Output
>Factorial of 5 is: 120




