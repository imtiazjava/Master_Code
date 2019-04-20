Program : FOP_1.
Language: Java
Level   : Basic
Module  : Fundamental of Programming
Topic   : Control Statements

Problem Statement : Sudeer wants to check his level of coding in basic to find out  sum of digits of the given two digit number. 
In order to find out this we have given method templet for you in that you need  to write the code by following specifications:


Specifications: The value returned by the method getSumOfdigits() is determined by the following rules:

if the given value is in between 10 and 99, return sum of it's digits. Example: if x = 34, return 7
if the given value is negative, return -3
if the given value is greater than 99, return -2
if the given value is in between 0 and 9, return -1

Input Format  : N is a positive integer value.

Output Format : Method should return sum of its digit of given number.

Constraints:
10<=N<=99

Sample Input1:
22
Sample Outptu1:
4
Sample Input2:
9

Sample Output2:
-1

Sample Input3:
-10
Sample Output3:
-3

Input4:
47
Output4:
11

Input5:
66
Output5:
12

Input6:
0
Output6:
-1

Input7:
99

Output7:
18
Input8:
1
Output8:
-1

Input9:
222

Output9:
-2

Input10:
1000

Output10:
-2

Templet:
========
 import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int no = sc.nextInt();
		System.out.println(getSumOfDigits(no));
	}

	public static int getSumOfDigits(int no) {
		int sum = 0;
		//write the code here 
		return sum;
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int no = sc.nextInt();
		System.out.println(getSumOfDigits(no));
	}

	public static int getSumOfDigits(int no) {
		int sum = 0;
		if (no >= 0 && no <= 9)
			return -1;
		else if (no > 99)
			return -2;
		else if (no < 0)
			return -3;
		else {
			sum = (no / 10) + (no % 10);
		}
		return sum;
	}
}
===============================================================================================================
Program : FOP_2 
Language: Java
Level   : Basic
Module  : Fundamental of Programming
Topic   : Control Statements

Can you write  a  method which is used to find out the  
difference of digits of the given two digit numbers by using following specifications.


Specifications: The value returned by the method findDiffOfdigits() is determined by the following rules:

If the given value is in between 10 and 99, return difference of it's digits. 
Example: 
if x = 83,  8 - 3 return 5. 
if x = 38, 3 - 8 return -5.
if the given value is negative, return -3
if the given value is greater than 99, return -2
if the given value is in between 0 and 9, return -1

Note: You should substract the units position value from tens positon value, the return value may be negative.

Constraints:
10<=N<=99

Sample Input1:
83
Sample Output2:
5

Sample Input2:
100
Sample Output2:
-2

Sample Input3:
-12
Sample Output3:
-3

Input4:
99
 
Output4:
0

Input5:
78

Output5:
-1

Input6:
90

Output6:
9

Input7:
61

Output7:
5

Input8:
21

Output8:
1

Input9:
10
Output9:
1

Input10:
-100
Output10:
-3


Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int no = sc.nextInt();
		System.out.println(findDiffOfdigits(no));
	}

	public static int findDiffOfdigits(int num) {
		   return 0;
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int no = sc.nextInt();
		System.out.println(findDiffOfdigits(no));
	}

	public static int findDiffOfdigits(int num) {
		if (num >= 0 && num < 10)
			return -1;
		if (num >= 100)
			return -2;
		if (num < 0)
			return -3;

		return (num / 10) - (num % 10);
	}
}
=====================================================================================

Program: FOP_3
Language: Java
Level   	   : Basic
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:  


For a given method write the logic which returns the 1 
if the given three digit number is palindrome, in other case return 0.

Specifications: The value returned by the method isPalindrome() is determined by the following rules:

if the given number is an three digit number, retun 1 if the number is palindrome, else return 0. Example: if x = 232, return 1. if x = 345, return 0
if the given number is negative or zero, return -1
if the given number is not an three digit number, return -2


Sample Input1  :
5555

Sample Output1 :
-2

Sample Input2:
555

Sample Output2:
1

Sample Input3:
-111

Sample Output3:
-1
 
Input4:
100

Output3:
0

Input5:
222

Output5:
1

Input6:
22

Output6:
-2

Input7:
151

Output7:
1

Input8:
909
Output8:
1

Input9:
212

Output9:
1

Input10:
767
Output10:
1

Templet:
========
import java.util.Scanner;

public class Test {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(isPalindrome(num));
	}

	public static int isPalindrome(int num) {
		   //write the code here.
	}

}

Solution:
=========
import java.util.Scanner;

public class Test {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(isPalindrome(num));
	}

	public static int isPalindrome(int num) {
		if (num <= 0)
			return -1;
		if (!(num >= 100 && num <= 999))
			return -2;
		if (num % 10 == num / 100)
			return 1;
		return 0;
	}

}
===================================================================================================
Program: FOP_4
Language: Java
Level   	   : Basic
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:  
For a given  method write a logic which returns  1 if the given number is even, in other case return 0.

Specifications : The value returned by the method isEven() is determined by the following rules:

if the given number is an even number, return 1 else return 0. 
Example 
if x = 22, return 1. 
if x = 35, return 0
if the given number is negative or zero, return -1

Constraints
1<=N<=2^31

Sample Input1:
10

Sample Output1:
1

Sample Output2:
11

Sample Output2:
0

Sample Input3:
-20
Sample Output3:
-1

Input4:
200
Output4:
1

Input5:
1001
Output5:
0

Output6:
786
Output6:
1

Input7:
294
Output7:
1

Input8:
981
Output8:
0

Input9:
1033
Output9:
0

Output10:
100000002

Output10:
1


Templet:
========
import java.util.Scanner;

class Test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        System.out.println(isEven(num));
    }
    
    public static int isEven(int num) {
			//write the code here.
    }
}

Solution:
=========
import java.util.Scanner;

class Test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        System.out.println(isEven(num));
    }
    
    public static int isEven(int num) {
        if (num <= 0)
            return -1;
        if (num % 2 == 0)
            return 1;
        return 0;
    }
}
===========================================================================
Program: FOP_5
Language: Java
Level   	   : Basic
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:  

For a given method write a logic  which returns the greatest number 
among two numbers by using following specifications.

Specifications: The value returned by the method getGreatest() is determined by the following rules:

if any of the given numbers are negative, return -1.
if any of the given numbers are zero, return -2.
if the given numbers are positive, return the greatest.

Input Format: You need to pass two inputs i.e. is N1 and N2 of type integer.

Output Format : Print Greatest number among two numbers.

Constraints
1<=N1<=10^31
2<=N2<=10^31


Sample Input1:
10 200

Sample Output1:
200

Sample Input2:
100 -200

Sample Output2:
-1

Sample Input3:
0 0
Sample Output3:
-2

Input4:
100 0

Output4:
-2

Input5:
202 222

Output5:
222

Input6:
1 1

Output6:
1

Input7:
-1 1

Output7:
-1

Input8:
0 0 

Output8:
-2

Input9:
99 999

Output9:
999

Input10:
111 111

Output10:
111


Templet:
========
import java.util.Scanner;

public class Test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n1 = sc.nextInt();
        int n2 = sc.nextInt();
        System.out.println(getGreatest(n1, n2));
    }

    public static int getGreatest(int num1, int num2) {
			//write the logic here.
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n1 = sc.nextInt();
        int n2 = sc.nextInt();
        System.out.println(getGreatest(n1, n2));
    }

    public static int getGreatest(int num1, int num2) {
        if (num1 < 0 || num2 < 0)
            return -1;
        if (num1 == 0 || num2 == 0)
            return -2;
        if (num1 > num2)
            return num1;
        return num2;
    }
}
====================================================================================
Program: FOP_6
Language: Java
Level   	   : Basic
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:  

For a given method write a logic which returns the least number among two numbers by using following specifications.
 
Specifications: The value returned by the method getLeastNum() is determined by the following rules:

if any of the given numbers are negative, return -1.
if any of the given numbers are zero, return -2.
if the given numbers are positive, return the least number.

Input Format: You need to pass two inputs i.e. is N1 and N2 of type integer.

Output Format : Print Least number among two numbers.

Constraints
1<=N1<=10^31
2<=N2<=10^31

Sample Input1:
100 200

Sample Output1:
100

Sample Input2:
-100 200

Sample Output2:
-1

Sample Input3:
100 0

Sample Output3:
-2

Input4:
0 0
Output4:
-2

Input5  :
0 -1 

Output5 :
-1

Input6:
90 99

Output6:
90

Input7:
100 -100

Output7:
-1

Input8:
10000 10001

Output8:
10000

Input9:
20001 000000

Output9:
-2

Input10:
8991 12221

Output10:
8991

Templet:
========
import java.util.Scanner;

public class Test {
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int n1 = sc.nextInt();
       int n2 = sc.nextInt();
        System.out.println(getLeastNum(n1, n2));
    }

    public static int getLeastNum(int num1, int num2) {
         //write the logic here.
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
       int n1 = sc.nextInt();
       int n2 = sc.nextInt();
        System.out.println(getLeastNum(n1, n2));
    }

    public static int getLeastNum(int num1, int num2) {
        if (num1 < 0 || num2 < 0)
            return -1;
        if (num1 == 0 || num2 == 0)
            return -2;
        if (num1 < num2)
            return num1;
        return num2;
    }
}
===========================================================================================
Program: FOP_7
Language: Java
Level   	   : Medium
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement: 

Write a method which accepts two value as arguments(an integer and boolean) and return the string indicating when the alarm should ring. 

the first argument indicating day of the week encoded as 
0=Sun, 1=Mon, 2=Tue, ...6=Sat, and a boolean indicating if we are on vacation or not.

 

Specifications: The value returned by the method ringAlarm() is determined by the following rules:

if the first argument value is not between 0 to 6, return "Invalid Inputs"
if the second value is not boolean value true or false, return "Invalid Inputs"
if the first argument value is between 1 to 5 indicating the week day's and second value is true indicating on vacation, return "10:00"
if the first argument value is between 1 to 5 indicating the week day's and second value is false indicating not on vacation, return "07:00"
if the first argument value is 0 or 6 indicating the weekend day's and second value is true indicating on vacation, return "OFF"
if the first argument value is 0 or 6 indicating the weekend day's and second value is false indicating not on vacation, return "OFF"


Input Format  : Take first value as integer i.e. is day_of_week, second value as boolean i.e. is onVacation.

Output Format : Print output in the form of string.

Sample Input1:
10 true

Sample Output1:
Invalid Input

Sample Input2:
1 true

Sample Output2:
10:00

Sample Input3:
1 false

Sample Output3:
07:00

Input4:
0 true

Output4:
OFF

Input5:
6 true

Output5:
OFF

Input6:
6 false

Output6:
OFF

Input7:
3 false

Output7:
07:00

Input8:
4 true

Output8:
10:00

Input9:
5 false

Output9:
07:00

Input10:
2 true

Output10:
10:00


Templet:
========
import java.util.Scanner;

public class Test {
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
    	int day_of_week = sc.nextInt();
        boolean onVac = sc.nextBoolean();
        System.out.println(ringAlarm(day_of_week, onVac));
    }

    public static String ringAlarm(int dayOfWeek, boolean onVac) {
			//write the code here.
    	 
    	
    }
}

Solution:
==========
import java.util.Scanner;

public class Test {
    public static void main(String[] args) {
       Scanner sc = new Scanner(System.in);
    	int day_of_week = sc.nextInt();
        boolean onVac = sc.nextBoolean();
        System.out.println(ringAlarm(day_of_week, onVac));
    }

    public static String ringAlarm(int dayOfWeek, boolean onVac) {
         
    	if(dayOfWeek<0 || dayOfWeek>6)
    		return "Invalid Input";
    	if(!(onVac==true || onVac==false))
    		return "Invalid Input";
    	if(onVac){
    			  if(dayOfWeek==0 || dayOfWeek==6)
    				  return "OFF";
    		return "10:00";
    	}else{
    			 if(dayOfWeek==0 || dayOfWeek==6)
    				 return "OFF";
    			 
    		return "07:00";
    	}
    	
    }
}
====================================================================================================================
Program: FOP_8
Language: Java
Level   	   : Hard
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

Teacher asked abdul rehman to write a program which Roman number to decimal.
Below teacher has given  example to find its corresponding decimal value.

Example :

Input : IX
Output : 9

Input : XL
Output : 40

Input : MCMIV
Output :  1904
M is a thousand, CM is nine hundred 
and IV is four


Roman numerals are based on below symbols.

SYMBOL       VALUE
I             1
IV            4
V             5
IX            9
X             10
XL            40
L             50
XC            90
C             100
CD            400
D             500
CM            900 
M             1000      

A number in Roman Numerals is a string of these symbols written in descending order(e.g. M’s first, followed by D’s, etc.). However, in a few specific cases, to avoid four characters being repeated in succession (such as IIII or XXXX), subtractive notation is often used as follows:

I placed before V or X indicates one less, so four is IV (one less than 5) and 9 is IX (one less than 10).
X placed before L or C indicates ten less, so forty is XL (10 less than 50) and 90 is XC (ten less than a hundred).
C placed before D or M indicates a hundred less, so four hundred is CD (a hundred less than five hundred) and nine hundred is CM (a hundred less than a thousand).

Sample Input1:
MCMIV

Sample Output1:
1904

Explanation:
M is a thousand, CM is nine hundred 
and IV is four

Sample Input2:
XI

Sample Output2:
11

Sample Input3:
xx

Sample Output3:
-2
 
Input4: 
IV

Output4:
4

Input5:
VII

Output5:
7

Input6:
VIII
Output6:
8

Input7:
XXC

Output7:
100

Input8: 
MCM

Output8:
1900

Input9:
XLL

Output9:
90

Input10:
XCCD
Output10:
490

Templet:
========
import java.util.Scanner;

public class Test {
	 
	public static void main(String args[]) {
		Scanner sc = new Scanner(System.in);
		String input = sc.next();
		System.out.println(romanToDecimal(input));

		 
	}
	 
		public static int value(char r) {
			 //write the code here
			return -1;
		}

	  	public static int romanToDecimal(String input) {
			// Initialize result
			int result = 0;
 			//write the code here.
			return result;
		}

}


Solution:
==========
import java.util.Scanner;

public class Test {
	 
	public static void main(String args[]) {
		Scanner sc = new Scanner(System.in);
		String input = sc.next();
		System.out.println(romanToDecimal(input));

		 
	}
	// This method returns value of a Roman symbol
		public static int value(char r) {
			if (r == 'I')
				return 1;
			if (r == 'V')
				return 5;
			if (r == 'X')
				return 10;
			if (r == 'L')
				return 50;
			if (r == 'C')
				return 100;
			if (r == 'D')
				return 500;
			if (r == 'M')
				return 1000;
			return -1;
		}

		// Finds decimal value of a given romal numeral
		public static int romanToDecimal(String input) {
			// Initialize result
			int result = 0;

			for (int i = 0; i < input.length(); i++) {
				// Getting value of symbol s[i]
				int s1 = value(input.charAt(i));

				// Getting value of symbol s[i+1]
				if (i + 1 < input.length()) {
					int s2 = value(input.charAt(i + 1));

					// Comparing both values
					if (s1 >= s2) {
						// Value of current symbol is greater
						// or equal to the next symbol
						result = result + s1;
					} else {
						result = result + s2 - s1;
						i++; // Value of current symbol is
						// less than the next symbol
					}
				} else {
					result = result + s1;
					i++;
				}
			}

			return result;
		}

}
=====================================================================================================
Program: FOP_9
Language: Java
Level   	   : Medium
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

Find total number of Squares in a N*N cheesboard.

Input:
The first line contains an integer T, depicting total number of test cases. 
Then following T lines contains an integer N that is the side of the chessboard.

Output:
Each seperate line showing the maximum number of squares possible.

Constraints:
1 <= T <= 100
1 <= N <= 100

Example:
Sample Input1:
2
1
2

Sample Output1:
1
5

Sample Input2:
3
1
2
3
Sample Output2:
1
5
14

Sample Input3:
1
4
Sample Output3:
30

Input4:
1
5
Output4:
55

Input5:
2
3
3

Output5:
14
14

Input6:
1
6
Output6:
91

Input7:
7
1
2
3
3
4
5
5
Output7:
1
5
14
14
30
55
55

Input8:
6
1
2
2
1
5
4

Output8:
1
5
5
1
55
30

Input9:
9
1
2
3
4
4
5
1
7
4

Output9:
1
5
14
30
30
55
1
140
30

Input10  :
2
4
4
Output10 :
30
30

Templet:
========

 
import java.util.Scanner;

class Test {
	public static void main(String[] args) {
	 
		Scanner sc = new Scanner(System.in);
		//write the code here.
		sc.close();
	}
}

Solution:
=========

 
import java.util.Scanner;

class Test {
	public static void main(String[] args) {
	 
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int index =0;
		int arr[] = new int[100];
		while (t != 0) {
			int no = sc.nextInt();
			int res = ((no * no + no) * (2 * no + 1)) / 6;
			 arr[index++]= res;

			t--;
		}
		for(int i=0;i<index;i++){
			System.out.println(arr[i]);
		}
		sc.close();
	}
}
=========================================================================================================
Program: FOP_10
Language: Java
Level   	   : Medium
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

Given two positive integers N and X, where N is the number of total patients and X is the time duration(in minutes) after which a new patient arrives. 
Also, doctor will give only 10 minutes to each patient. 
The task is to calculate the time (in minutes) the last patient needs to wait.

Input:
The first line of input contains the number of test cases T. 
The next subsequent lines denote the total number of patients N and time interval X(in minutes) in which the next patients are visiting.

Output:
Output the waiting time of last patient.

Constraints:
1 <= T <= 100
0 <= N <= 100
0 <= X <= 30

Example:
Sample Input1:
5
4 5
5 3
6 5
7 6
8 2

Sample Output1:
15
28
25
24
56

Sample Input2:
2
5 5
5 4

Sample Output2:
20
24

Sample Input3 :
1
4 4
Sample Output3:
18

Input4:
2
5 4
10 10

Output4:
24
0

Input5:
3
5 5
4 4 
11 111
Output5:
20
18
0

Input6:
4
1 1
2 2
3 4
4 4

Output6:
0
8
12
18

Input7:
5
1 2
2 3
3 4
4 5
5 6

Output7:
0
7
12
15
16

Input8:
6
6 6
5 5
4 4
3 3
2 2
1 1
Output8:
20
20
18
14
8
0

Input9:
1
9 9

Output9:
8

Input10:
3
33 3
11 1
2 2
Output10:
224
90
8


Templet:
=========
import java.util.Scanner;

class Test {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		//write the code here.
			 
		sc.close();
	}

}

Solution:
=========
import java.util.Scanner;

class Test {
	public static void main(String[] args) {
		// code
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int arr[] = new int[t];
		int index =0;
		int total = 0;
		while (t != 0) {
			int N = sc.nextInt();
			int X = sc.nextInt();
			if (X < 10) {
				total = (10 - X) * (N - 1);
				 
			}else {
				total = 0;
			}
			arr[index++] = total;
			t--;

		}
		for(int i=0;i<index;i++){
		 
			System.out.println(arr[i]);
		}
		sc.close();
	}

}
=====================================================================================================
Program: FOP_11
Language: Java
Level   	   : Easy
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

Given a positive integer n, check if it is perfect square or not.
Note: Try to solve the question using only addition and subtraction operation.

Input:
The first line of input contains an integer T denoting the number of test cases. 
Then T test cases follow. The first line of each test case contains an integer the integer n.

Output:
Print 1 if n is a perfect square else print 0. 
Print the answer for all test case in a new line.

Constraints:
1<= T <=100
1<= N <=100000
Hint:
Addition of first n odd numbers is always perfect square 
1 + 3 = 4,      
1 + 3 + 5 = 9,     
1 + 3 + 5 + 7 + 9 + 11 = 36 ...
Example:
Sample Input1:
2
35
49
Sample Output1:
0
1

Sample Input2:
1
36

Sample Output2:
1

Sample Input3:
3
9
25
55
Sample Output3:
1
1
0

Input4:
5
1
2
3
4
5
Output4:
1
0
0
1
0

Input5:
2
1000
2080
Output5:
0
0

Input6:
6
10
20
30
40
50
60
Output6:
0
0
0
0
0
0
Input7:
8
111
213
333
414
555
515
666
616
Output7:
0
0
0
0
0
0
0
0

Input8:
3
300000
10000
200000

Output8:
0
1
0
Input9:
5
999
888
777
666
555
Output9:
0
0
0
0
0
Input10:
1
1
Output10:
1

Templet:
========
import java.util.Scanner;

class Test {
	static boolean isPerfectSquare(int n) {
		//write the code here.
	}

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		 //write the code here
		 sc.close();
	}
}

Solution:
========
import java.util.Scanner;

class Test {
	static boolean isPerfectSquare(int n) {
		for (int sum = 0, i = 1; sum < n; i += 2) {
				sum += i;
			if (sum == n)
				return true;
		}
		return false;
	}

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int arr[] = new int[t];
		int index = 0;
		for (int i = 1; i <= t; i++) {
			int no = sc.nextInt();
			if (isPerfectSquare(no)) {
				arr[index++] = 1;
			} else {
				arr[index++] = 0;
			}

		}
		for (int a : arr) {
			System.out.println(a);
		}
	}
}
==================================================================================================
Program: FOP_12
Language: Java
Level   	   : Easy
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

 
 
Given an integer N, denoting the number of cuts that can be made on a pancake, find the maximum number of pieces that can be formed by making N cuts.

Input:
The first line of input contains a single integer T denoting the number of test cases. 
Then T test cases follow. Each test case consist of one line. The first line of each test case consists of an integer N.

Output:
Corresponding to each test case, in a new line, print the maximum number of pieces that can be formed by making N cuts .

Constraints:

1 ≤ T ≤ 50
1 ≤ N ≤ 10^3

Example:
Sample Input1 :
2
5
3
Sample Output1 :
16
7

Sample Input2:
1
4

Sample Output2:
11

Sample Input3:
3
1
2
3

Sample Output3:
2
4
7
Input4:
4
11
21
22
33
Output4:
67
232
254
562

Input5:
3
2
2
2

Input5:
4
4
4

Input6:
6
21 
12
32
23
45
56
Output6:
232
79
529
277
1036
1597

Input7:
8
11
100
200
333
444
555
22
11

Output7:
67
5051
20101
55612
98791
154291
254
67

Input8:
10
1
22
33
44
5555
66
77
88
999
22
Output8:
2
254
562
991
15431791
2212
3004
3917
499501
254

Input9:
2
10000
200

Output9:
50005001
20101

Input10:
4
90
80
70
60
Output10:
4096
3241
2486
1831

Templet:
========
import java.util.Scanner;
/*
 * 
 * We now know ,
f(n) = n + f(n-1) 

Expanding f(n-1) and so on we have ,
f(n) = n + n-1 + n-2 + ...... + 1 + f(0)

which gives,
f(n) = (n*(n+1))/2 + 1
 */
class Test {
	public static void main(String[] args) {
		  //write the logic here.
	}
}

Solution:
========
import java.util.Scanner;
class Test {
	public static void main(String[] args) {
		 Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		long arr[] = new long[t];
		int index = 0;
		while (t != 0) {
			int N = sc.nextInt();
		 	int result = (N*(N+1))/2 +1;
			arr[index++] = result;
			t--;
		}
		for (int i = 0; i < index; i++)
			System.out.println(arr[i]);
		sc.close();
	}
}
===============================================================================================================
Program: FOP_13
Language: Java
Level   	   : Easy
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

You are given an integer input N and you have to find whether it is Anshuman’s favourite or not.

If it is then print "YES" else print "NO".

A number is Anshuman’s favourite if it is either the sum or the difference of the integer 5. (5+5, 5+5+5, 5-5,5-5-5+5+5…..)

Input:
The first line of input contains an integer denoting the number of test cases . Next line of input contains an integer N to be tested.    

Output:
For each test case , the output is in a new line containing the answer 'YES' or 'NO' depending on whether the given number N is Anshuman's favourite or not .

Constraints:
1<=T<=100
-10^9<=N<=10^9

Example:
Input : 
1
10
Output : 
YES

Because 10 can be written as a sum of 5+5.

Example:
Sample Input1: 
1
9
Sample Output1: 
NO

Sample Input2:
2
-255
389
Sample Output2:
YES
NO

Sample Input3:
3
100
230
999

Sample Output3:
YES
YES
NO

Input4:
2
878
211
Output4:
NO
NO

Input5:
6
1
2
3
33
44
50
Output5:
NO
NO
NO
NO
NO
YES

Input6:
3
10
20
30
Output6:
YES
YES
YES

Input7:
2
10001
20001
Output7:
NO
NO

Input8:
4
22
44
55
10

Output8:
NO
NO
YES
YES

Input9:
2
100
-200

Output9:
YES
YES

Input10:
2
101
-200
Output10:
NO
YES

Input11:
2
-100
-200
Output11:
YES
YES

Templet:
=========
 
import java.util.Scanner;

class Test {
	public static void main (String[] args) {
		 //write the code here..
	}
}

Solution:
=========
 
import java.util.Scanner;

class Test {
	public static void main (String[] args) {
		//code
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		String s[] = new String[t];
		int index =0;
		while(t!=0){
		    int N = sc.nextInt();
		    if(N%5==0){
		        s[index++] ="YES";
		    }else {
		        s[index++] = "NO";
		    }
		    
		    t--;
		}
		for(int i=0;i<index;i++){
		    System.out.println(s[i]);
		}
	}
}
============================================================================================
Program: FOP_14
Language: Java
Level   	   : Easy
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   


Given a non-negative integer num, repeatedly add all its digits until the result has only one digit.

Input:
The first line contains 'T' denoting the number of testcases. Then follows description of testcases. The next T lines contains a single integer N denoting the value of N.


Output:
Output the sum of all its digit until the result has only one digit.


Constraints:
1<=T<=30
1<=n<=10^9


Example:
Sample Input1:
2
1
98
Sample Output1:
1
8

Explanation:For example, if we conisder 98, we get 9+8  = 17 after first addition. Then we get 1+7 = 8.  We stop at this point because we are left with one digit.


Sample Input2:
3
1
8
20
Sample Output2:
1
8
2

Sample Input3:
1
122
Sample Output3:
5

Input4:
3
99
999
1000
Output4:
9
9
1

Input5:
2
87
1
Output5:
6
1

Input6:
5
12
77
99
00
11
Output6:
3
5
9
0
2
Input7:
3
100
200
300
Output7:
1
2
3

Input8:
6
22
345
66
88
33

Output8:
1
4
3
3
7
6
1

Input9:
4
111
222
333
444
Output9:
3
6
9
3

Input10:
4
1212
121212
12121212
1212121212
Output10:
6
9
3
6

Templet:
========

import java.util.Scanner;

class Test {
	public static int sumOfDigits(int no) {
		 //write the code here.
	}

	public static void main(String[] args) {
		 //write the code here.
	}
}

Solution:
=========

import java.util.Scanner;

class Test {
	public static int sumOfDigits(int no) {
		int sum = 0;
		while (no != 0) {
			sum+= no % 10;
			no = no / 10;
		}
		if (sum >9) {
			sum=sumOfDigits(sum);
		}
		return sum;
	}

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int arr[] = new int[t];
		int index = 0;
		while (t != 0) {
			int N = sc.nextInt();
			arr[index++] =sumOfDigits(N);
			t--;
		}
		for (int i = 0; i < index; i++) {
			System.out.println(arr[i]);
		}
		sc.close();
	}
}
==========================================================================================================================
Program: FOP_15
Language: Java
Level   	   : Medium
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   

 Sherlock Being tired with the usual coding rounds started growing his interest towards reverse coding when he won the event in his college symposium. 
 He wondered if his friend has the brain to quickly identify the pattern and verify if his inputs are correct or not. 
 From the example portion given below, where you will be given a number(n) and its output, Using this find the pattern. 
 Your task is that from the pattern you identified above, You have to tell if for the given n whether the given m is the correct answer or not.

Input:
The first line consists of T, the number of test cases. then T lines follow. Each line consists of n and m.

Output:
For each n and m output 1 if m is the corresponsing input for the value of n and 0 otherwise.

Constraints:
1<=t<=50
0<=n<=1000
0<=m<=10^6

Example to identify the pattern :

Input                            Output

10                                 55

20                                 210

5                                   15

0                                    0

1                                    1

2                                    3

Example:
Sample Input1:
4
10 55
4  11
2  3
6  21

Sample Output1:
1
0
1
1

Sample Input2:
2
20 210
5 16

Sample Output2:
1
0


Sample Input3:
5
0 0
1 1
2 3
3 3
4 4
Sample Output3:
1
1
1
0
0

Input4:
2
121 1333
122 121
Output4:
0
0

Input5:
3
25 325
33 561
270 36585

Output5:
1
1
1

Input6:
2
11 66
44 990
Output6:
1
1

Input7:
4
80 3241
90 4095
100 5051
110 6105

Output7:
0
1
0
1

Input8:
3
141 10011
151 11476
131 8646
Output8:
1
1
1
Input9:
3
11 111
12 121
13 131
Output9:
0
0
0

Input10:
1
1 1
Output10:
1

Templet:
========
 
import java.util.Scanner;

class Test {
	public static void main (String[] args) {
		//write the code here.	 
		 
    }
}

Solution:
=========
import java.util.Scanner;

class Test {
	public static void main (String[] args) {
		Scanner sc = new Scanner(System.in);
		int t = sc.nextInt();
		int arr[] = new int[t];
		int index =0;
		while(t--!=0){
		    int n = sc.nextInt();
		    int m = sc.nextInt();
		      if((n*(n+1)/2)==m)
		        arr[index++]=1;
		      else
		        arr[index++]=0;
		}
		for(int i=0;i<index;i++)
		    System.out.println(arr[i]);
		
		sc.close();
	}
}
==================================================================================================================================
Program		: FOP_16
Language	: Java
Level   	: Hard
Module   	: Fundamental of Programming
Topic       : Control Statements
Problem Statement:   

A number n is said to be Deficient Number if sum of all the divisors of the number denoted by divisorsSum(n) is less than twice the value of the number n. 
And the difference between these two values is called the deficiency.

Mathematically, if below condition holds the number is said to be Deficient:

divisorsSum(n) < 2 * n
deficiency = (2 * n) - divisorsSum(n)
The first few Deficient Numbers are:

1, 2, 3, 4, 5, 7, 8, 9, 10, 11, 13, 14, 15, 16, 17, 19 …..

Given a number n, our task is to find if this number is Deficient number or not.

Examples :

Input: 21
Output: 1
Divisors are 1, 3, 7 and 21. Sum of divisors is 32.
This sum is less than 2*21 or 42.

Input:
The first line of input contains an integer T denoting the no of test cases.
Then T test cases follow. Each line contains an integer x.

Output:
For each test case in a new line print 1 if the no is a Deficient number else print 0.

Constraints:
1<=T<=10000
1<=x<=10000


Example:
Sample Input1:
3
21
12
17
Sample Output1:
1
0
1

Sample Input2:
1
6
Sample Output2:
0

Sample Input3:
2
7
10
Sample Output3:
1
1
Input4:
4
13
14
14
20
Output4:
1
1
1
0
Input5:
5
21
22
31
33
41
Output5:
1
1
1
1
1
Input6:
6
31
33
34
35
38
39
Input6:
1
1
1
1
1
1
Input7:
1
20001
Output7:
1
Input8:
2
2002
12021
Output8:
0
1
Input9:
4
3001
2001
1001
4001
Output9:
1
1
1
1
Input10:
8
8001
7007
8008
6666
3333
2222
1111
9999
Output10:
1
1
0
0
1
1
1
1

Templet:
========

import java.util.Scanner;

class Test {

	public static void main(String[] args) {
	   	 
    }
    
}

Solution:

import java.util.Scanner;

class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int T = sc.nextInt();
		int arr[] = new int[T];
		int index = 0;
		while (T != 0) {
			int x = sc.nextInt();
			if (isDeficient(x)) {
				arr[index++] = 1;
			} else {
				arr[index++] = 0;
			}
			T--;
		}
		for (int i = 0; i < index; i++) {
			System.out.println(arr[i]);
		}
	}

	// Function to check Deficient Number
	static boolean isDeficient(int n) {
		// Check if sum(n) < 2 * n
		return (divisorsSum(n) < (2 * n));
	}

	static int divisorsSum(int n) {
		int sum = 0; // Initialize sum of prime factors

		// Note that this loop runs till square root of n
		for (int i = 1; i <= (Math.sqrt(n)); i++) {
			if (n % i == 0) {
				// If divisors are equal, take only one
				// of them
				if (n / i == i) {
					sum = sum + i;
				} else // Otherwise take both
				{
					sum = sum + i;
					sum = sum + (n / i);
				}
			}
		}

		return sum;
	}

}
=====================================================================================================================================================
Program   : FOP_17
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   
   

You will be given a positive integer K. Your task is to find the number of ordered pairs of positive integers (a,b) where 1 ≤ a < b < K such that a + b ≤ K.
Input: 
The first line of input contains a single integer T denoting the number of test cases.
Then T test cases follow. The first and only line of each test case consists of K.
 

Output:
Corresponding to each test case, in a new line, print the number of ordered pairs of positive integers (a,b) where 1 ≤ a < b < K such that a + b ≤ K.

 

Constraints:
1 ≤ T ≤ 100
1 ≤ K ≤ 1000
 
Explanation: 
For K = 4, the two ordered pairs are (1,2) and (1,3). 
For K = 5, the four ordered pairs (1,2), (1,3), (1,4) and (2,3). 

Example:

Sample Input1:
3
2
4
5
Sample Output1:
0
2
4

Sample Input2:
1
5
Sample Output2:
4

Sample Input3:
1
4
Sample Output3:
2

Input4:
2
3
2
Output4:
1
0
Input5:
3
1
2
3
Output5:
0
0
1
Input6:
4
5
5
6
6
Output6:
4
4
6
6
Input7:
3
7
8
9
Output7:
9
12
16
Input8:
6
1
2
3
4
5
6
Output8:
0
0
1
2
4
6
Input9:
2
8
7
Output9:
12
9
Input10:
1
1
Output10:
0

Templet:
========
 
import java.util.Scanner;

class Test {
	public static void main (String[] args) {
		 //write the logic here..
	}
}

Solution:
=========
 
import java.util.Scanner;

class Test {
	public static void main (String[] args) {
		Scanner sc = new Scanner(System.in);
		 int t = sc.nextInt();
		 int arr[] = new int[t];
		 int index =0;
		 while(t-- > 0){
		     int K = sc.nextInt();
		     int count = 0;
		     int n = K%2==0 ? (K/2)-1 : K/2;
		     for(int i=1; i<=n; i++){
		         for(int j=2; j<K; j++){
		             if(((i+j) <= K) && (i < j)){
		                 count++;
		             }
		         }
		     }
		     arr[index++] =count;
		 }
		 for(int i=0;i<index;i++){
			 System.out.println(arr[i]);
		 }
	}
}
==============================================================================================================================================================
Program   : FOP_18
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements & String
Problem Statement:   


John wants to put all natural numbers between a range of  two numbers 
in a string by maintaining a single space.
Note : Should not use loops.

Specification of method : 
 
Values must not be negative. If yes, then return -1 as string.                                
Values must not be 0. If yes, then return -2 as string. 
Natural Numbers must be returned as one string with every value separated by single blankspace.
Consider that, the first argument value is less than the second argument number. otherwise return empty string. 

Constraints:
1<=N1<=10^3
1<=N2<=10^3


Sample Input1:
1 10
Sample Output1:
1 2 3 4 5 6 7 8 9 10

Sample Input2:
10 1
Sample Output2:

Sample Input3:
-1 10
Sample Output3:
-1

Input4:
0 10
Output4:
-2

Input5:
1 5
Output5:
1 2 3 4 5

Input6:
2  12
Output6:
2 3 4 5 6 7 8 9 10 11 12

Input7:
10 20
Output7:
10 11 12 13 14 15 16 17 18 19 20
Input8:
1 1
Output8:
1
Input9:
999 1000
Output9:
999 1000
Output10:
990 1000
Output10:
990 991 992 993 994 995 996 997 998 999 1000

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
	 Scanner sc = new Scanner(System.in);
	 int num1 = sc.nextInt();
	 int num2 = sc.nextInt();
	 System.out.println(getNaturalNumbers(num1, num2));
	}

	public static String getNaturalNumbers(int num1, int num2) {
		String result = "";
 		//write the code here..
		return result.trim();
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
	 Scanner sc = new Scanner(System.in);
	 int num1 = sc.nextInt();
	 int num2 = sc.nextInt();
	 System.out.println(getNaturalNumbers(num1, num2));
	}

	public static String getNaturalNumbers(int num1, int num2) {
		String result = "";

		if (num1 < 0 || num2 < 0)
			return "-1";
		else if (num1 == 0 || num2 == 0)
			return "-2";
		else if (num1 <= num2) {
			if (num1 != num2)
				result += num1 + " ";
			else
				result += num1;
			return result += getNaturalNumbers(++num1, num2);
		} 

		return result.trim();
	}
}
=========================================================================================
Program   : FOP_19
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements & String
Problem Statement:   


John and smith are good programmers, 
every time smith give challange to John to solve problems, but know
John given challenge to smith to resolve whether a given number is kaprekar number or not.

In mathematics, a Kaprekar number for a given base is a non-negative integer, the representation of whose square in that base can be split into two parts that add up to the original number again. 
For instance, 45 is a Kaprekar number, because 45² = 2025 and 20 + 25 = 45.
For instance, 297 is a Kaprekar number, because 297² = 88209 and 88+209 = 297.
This are the kaprekar numbers 1, 9, 45, 55, 99, 297, 703, 999, 2223, 2728, 4879, 4950, 5050, 5292, 7272, 7777, 9999 etc.

Additional to that John given method to solve it the above problem by following specification:

If the given number is negative, return "-1" as string
If the given number is zero, return "-2" as string
in other case return "True" if it is a Kaprekar Number, else return "False".


Constraints:
1<=N<=10^4


Sample Input1:
45

Sample Output1:
True

Sample Input2:
-297
Sample Output2:
-1

Sample Input3:
0
Sample Output3:
-2

Input4:
1
Output4:
True

Input5:
11
Output5:
False

Input6:
13
Input6:
False

Input7:
20
Output7:
False

Input8:
4950
Output8:
True

Input9:
5050
Output9:
True

Input10:
7777
Output10:
True


Templet:
========
import java.util.Scanner;

class Test {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(iskaprekar(num));
	}

 	public static String iskaprekar(int num) {
		 //write the logic here..
	
	}

}

Solution:
=========
import java.util.Scanner;

class S {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(iskaprekar(num));
	}

 	public static String iskaprekar(int num) {
		if (num < 0)
			return "-1";
		if (num == 0)
			return "-2";
		if (num == 1)
			return "True";

		int sq_num = num * num;
		int count_digits = 0;
		while (sq_num != 0) {
			count_digits++;
			sq_num /= 10;
		}

		sq_num = num * num; 

		for (int r_digits = 1; r_digits < count_digits; r_digits++) {
			int eq_parts = (int) Math.pow(10, r_digits);

			if (eq_parts == num)
				continue;

			int sum = sq_num / eq_parts + sq_num % eq_parts;
			if (sum == num)
				return "True";
		}

	 
		return "False";
	}
}
==============================================================================================================================
Program   : FOP_20
Language : Java
Level   	   :  Easy
Module   : Fundamental of Programming
Topic        : Control Statements & String
Problem Statement:   
 

Mr. Horner wants to write a method which can check whether a given input is a prime number or not by following

method specification:

Name of method : checkPrime(static method)
Arguments      : 1 Integer Argument 
Return Type    : A String value

Value must not be negative. If yes, then return -1 as string.
Value must not be 0 or 1. If yes, then return -2 as string.
If value is a prime number, then return true as string otherwise return false as string.


Constraints:
2<=N<=10^3

Sample Input1:
2
Sample Output1:
true

Sample Input2:
-5
Sample Output2:
-1

Sample Input3:
0
Sample Output3:
-2

Input4:
21

Output4:
false

Input5:
23
Output5:
true

Input6:
67
Output6:
true

Input7:
282
Output7:
false

Input8:
283
Output8:
true

Input9:
811
Output9:
true

Input10:
727
Output10:
true


Templet:
========
import java.util.Scanner;

public class Test {
	
	public static void main(String[] args) {
		 
	}
	
	 
}

Solution:
=========
import java.util.Scanner;

public class Test {
	
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num =sc.nextInt();
		System.out.println(checkPrime(num));
	}
	
	public static String checkPrime(int num) {
		String result = "true";

		if (num < 0)
			result = "-1";
		else if (num == 0 || num == 1)
			result = "-2";
		else {
			for (int i = 2; i <= num / 2; i++) {
				if (num % i == 0) {
					result = "false";
					return result;
				}
			}

		}

		return result;
	}
}
=============================================================================================================
Program   : FOP_21
Language : Java
Level   	   :  Easy
Module   : Fundamental of Programming
Topic        : Control Statements
Problem Statement:   


For a given method which accepts a value as number and returns the sum of factors of given number.

Specifications: The value returned by the method getSumOfFactors() is determined by the following rules:
Value must not be negative. If yes, then return -1
Value must not be 0. If yes, then return -2.
otherwise, return the sum of factors of a given number.

Constraints:
1<=N<=10^3

Sample Input1:
6
Sample Output1:
12
Sample Input2:
-7
Sample Output2:
-1
Sample Input3:

Sample Output3:
0
-2

Input4:
8
Output4:
15
Input5:
10
Output5:
18

Input6:
11
Output6:
12

Input7:
84
Output7:
224

Input8:
100
Output8:
217

Input9:
513
Output9:
800

Input10:
999
Output10:
1520

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(getSumOfFactors(num));
	}

	public static int getSumOfFactors(int num) {
		  //write the code here....
	}

}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(getSumOfFactors(num));
	}

	public static int getSumOfFactors(int num) {
		int result = 0;

		if (num < 0)
			result = -1;
		else if (num == 0)
			result = -2;
		else {
			for (int i = 1; i <= num; i++) {
				if (num % i == 0)
					result += i;
			}
		}

		return result;
	}

}
==================================================================================================================================================
Program   : FOP_22
Language : Java
Level   	   :  Easy
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   


For a given method which accepts a value as number and returns the count of factors of given number.
Example:
=========
111 is a number factor of given number is 1,3,37,111. Therefore count is 4.

Specifications: The value returned by the method getCountOfFactors() is determined by the following rules:
Value must not be negative. If yes, then return -1
Value must not be 0. If yes, then return -2.
otherwise, return the sum of factors of a given number.

Constraints:
1<=N<=10^3

Sample Input1:
4
Sample Output1:
3
Sample Input2:
-10
Sample Output2:
-1
Sample Input3:
0
Sample Output3:
-2

Input4:
111
Output4:
4

Input5:
117
Output5:
6

Input6:
126
Output6:
12

Input7:
144
Output7:
15

Input8:
168
Output8:
16

Input9:
180
Output9:
18

Input10:
999
Output10:
8

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(getSumOfFactors(num));
	}

	public static int getSumOfFactors(int num) {
		int count = 0;
 			//write the code here...

		return count;
	}

}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(getSumOfFactors(num));
	}

	public static int getSumOfFactors(int num) {
		int count = 0;

		if (num < 0)
			return  -1;
		else if (num == 0)
			return -2;
		else {
			for (int i = 1; i <= num; i++) {
				if (num % i == 0)
					count++;
			}
		}

		return count;
	}

}
===============================================================================================================================
Program   : FOP_23
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   


For a given method which accepts 3 values as number and checks and returns the name of the type of triangle generated.
 
Specification :  The value returned by the method findTriangle() is determined by the following rules:

Values must not be 0. If yes, then return -1 as string.                                                              
Values must not be negative. If yes, then return  -2 as string.                                 
Sum of two sides must be greater than the third side. If no, then return -3 as string
If its a triangle with valid sides, then return as string  whether the triangle formed is EQUILATERAL, ISOSCELES or SCALENE.

Constraints:
1<=N1<=100
1<=N2<=100
1<=N3<=100

Sample Input1:
3 3 3
Sample Output1:
EQUILATERAL

Sample Input2:
3 -3 2
Sample Output2:
-2

Sample Input3:
3 0 3
Sample Output3:
-1

Input4:
3 6 3
Output4:
-3

Input5:
3 3 2
Output5:
ISOSCELES

Input6:
21 20 15

Output6:
SCALENE

Input7:
21 14 24
Output7:
SCALENE

Input8:
99 99 99
Output8:
EQUILATERAL

Input9:
66 65 65
Output9:
ISOSCELES

Input10:
100 200 300
Output10:
-3

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num1 = sc.nextInt();
		int num2 = sc.nextInt();
		int num3 = sc.nextInt();
		System.out.println(findTriangle(num1,num2,num3));
	}

	public static String findTriangle(int num1, int num2, int num3) {
		 
	}

}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num1 = sc.nextInt();
		int num2 = sc.nextInt();
		int num3 = sc.nextInt();
		System.out.println(findTriangle(num1,num2,num3));
	}

	public static String findTriangle(int num1, int num2, int num3) {
		String result = "";

		if (num1 == 0 || num2 == 0 || num3 == 0)
			result = "-1";
		else if (num1 < 0 || num2 < 0 || num3 < 0)
			result = "-2";
		else {
			if ((num1 + num2 <= num3) || (num2 + num3 <= num1) || (num1 + num3 <= num2))
				result = "-3";
			else if ((num1 == num2) && (num2 == num3))
				result = "EQUILATERAL";
			else if ((num1 == num2) || (num2 == num3) || (num1 == num3))
				result = "ISOSCELES";
			else
				result = "SCALENE";
		}

		return result;
	}

}
============================================================================================================================
Program   : FOP_24
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   


Victor want to write a program to check the given number is and adam number are not.

Explanation:
If a number when reversed, the square of the number and the square of the reversed number should be number which are reverse to each other, is Adam number.
Example: 
Input: 12
12 ^ 2 = 144
21 ^ 2 = 441
The reverse of 144 is equal to 441 and reverse of 441 is equal to 144 so., 12 is an Adam number.
11, 12, 13, 21, 22, 31, 101, 102, 103, 111, 112, 113, 121 ... are Adam numbers.

Write the methods with the following specifications: 

Name of method isAdamNumber() // which accepts an integer as argument and return true if it is an adam number else return false.
Arguments: One argument an integer value
Return Type: an boolean value

Example:
Input: 121
Output: true

Input: 17
Output: false

Name of method getReverse() // which accepts an Integer value as argument and return the reverse of it.
Arguments: One argument of integer value
Return Type: an integer value

Example:
Input: 421
Output: 124

Input: 134
Output: 431

Name of method getSquare() // which accepts an Integer value as argument and square of the number
Arguments: One argument of integer value
Return Type: an integer value

Example:
Input: 12
Output: 144

Input: 36
Output: 1296


Constraints:
1<=N<=10^3

Sample Input1:
12
Sample Output1:
true

Sample Input2:
2
Sample Output2:
true
Sample Input3:
-12
Sample Output3:
false

Input4:
111
Output4:
true

Input5:
202
Output5:
true

Input6:
221
Output6:
true

Input7:
999
Output7:
false

Input8:
987
Output8:
false

Input9:
654
Output9:
false

Input10:
345
Output10:
false

Templet:
========
import java.util.Scanner;

class Test {
    public static void main(String[] args) {
         
    }
    
}

Solution:
=========
import java.util.Scanner;

class Test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int num =sc.nextInt();
        System.out.println(isAdamNumber(num));
    }

    public static boolean isAdamNumber(int num) {
        int square_num1 = getSquare(num);
        int square_num2 = getSquare(getReverse(num));
        if (square_num1 == getReverse(square_num2))
            return true;
        return false;
    }

    public static int getReverse(int n) {
        int rev_num = 0;
        while (n > 0) {
            int r = n % 10;
            rev_num = rev_num * 10 + r;
            n /= 10;
        }
        return rev_num;
    }

    public static int getSquare(int n) {
        return n * n;
    }
}
=======================================================================================================================
Program   : FOP_25
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   

In a given method write a logic to return true if sum of alternate digits is same otherwise return false.

Example:1

12345

1 + 3 + 5 = 9
2 + 4 = 6

As 9 is not equal to 6 return false
 

Example:2

15345

1 + 3 + 5 = 9
5 + 4 = 9

As 9 is equal to 9 return true
 
Method should meet the following functional expectations

1. Return true if two sums of alternate digits is same otherwise return false
2. If a number is negative or zero then return false.


Sample Input1:
15345
Sample Output1:
true

Sample Input2:
-15345
Sample Output2:
false

Sample Intput3:
0
Sample Output3:
false

Input4:
231
Output4:
true

Input5:
111
Output5:
false

Input6:
1431
Output6:
false

Input7:
1889
Output7:
false

Input8:
1000
Output8:
false

Input9:
202
Output9:
false

Input10:
555
Output10:
false

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(isSameSum(num));

	}

	public static boolean isSameSum(int n) {
		   //write the logic here...
		}
	}

}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(isSameSum(num));

	}

	public static boolean isSameSum(int n) {
		int sum1 = 0;
		int sum2 = 0;
		int count = 1;
		int r = 0;
		if (n <= 0)
			return false;
		else {
			while (n != 0) {
				r = n % 10;
				if (count % 2 == 0)
					sum1 = sum1 + r;
				else
					sum2 = sum2 + r;
				n = n / 10;
				count++;
			}

			return sum1 == sum2;
		}
	}

}
========================================================================================================
Program   : FOP_26
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   


For a given method find out the  Russian multiplication.

Russian Multiplication Explained:

The Russian multiplication, also called the Russian peasant algorithm, uses a halving and doubling method to multiply whole numbers

When halving, disregard any remainder. Just put the quotient in the halving column

When the number in the halving column is 1, cross out all rows that have an even number in the halving column

the answer is found by adding the remaining numbers in the doubling column

Example # 1: 11 × 12 

Halving                              Doubling

   11                    ×                  12 

   5                      ×                  24 

   2                      ×                  48  ---> Disregard this since 2 is even

   1                      ×                  96 


The product of 11 and 12 is: 12 + 24 + 96 = 132 

Constraints
1<=N1<=10^3
1<=N2<=10^3


If numbers are negative or zero, then return -1. 
Otherwise return the product of the two numbers. 


Sample Input1:
11 12

Sample Output1:
132

Sample Input2:
-11 -12

Sample Output2:
-1
 
Sample Input3:
0 0
Sample Output3:
-1

Sample Input4:
11 0
Sample Output4:
-1

Sample Input5:
0 12
Sample Output5:
-1

Sample Input6:
13 14
Sample Output6:
182

Sample Input7:
21 22
Sample Output7:
462

Sample Input8:
112 110
Sample Output8:
12320

Sample Input9:
150 200
Sample Output9:
30000

Sample Input10:
20 200
Sample Output10:
4000


Templet:
========
import java.util.Scanner;

public class Test {
	
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int N1 = sc.nextInt();
		int N2 = sc.nextInt();
		System.out.println(getProduct(N1, N2));
	}

	public static int getProduct(int num1, int num2) {
		  //write the logic here
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {
	
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int N1 = sc.nextInt();
		int N2 = sc.nextInt();
		System.out.println(getProduct(N1, N2));
	}

	public static int getProduct(int num1, int num2) {
		int sum = 0;

		if (num1 <= 0 || num2 <= 0) {
			return -1;
		}

		while (num1 > 0) {
			if (num1 % 2 != 0) {
				sum = sum + num2;
			}
			num2 = num2 * 2;
			num1 = num1 / 2;
		}

		return sum;
	}
}
====================================================================================
Program   : FOP_27
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements  & String
Problem Statement:   



For a given method write the logic which returns  Collatz Sequence for a give input value.
 

Specifications: The value returned by the method getCollatzSequence() is determined by the following rules:

If the given value is 5, return a string of Collatz Sequence as 5 16 8 4 2 1
If the given value is negative or zero then return "Error"

Note:
At each stage you must add the numbers to the output string and form the output.
The numbers in the output string must be separated by a space.
The output must include the given number and 1.
 
Constraints
1<=N<=10^3


Sample Input1:
5
Sample Output1:
5 16 8 4 2 1

Sample Input2:
-5
Sample Output2:
Error

Sample Input3:
0
Sample Output3:
Error

Input4:
12
Output4:
12 6 3 10 5 16 8 4 2 1

Input5:
8
Output5:
8 4 2 1

Input6:
20
Output6:
20 10 5 16 8 4 2 1

Input7: 
100
Output7:
100 50 25 76 38 19 58 29 88 44 22 11 34 17 52 26 13 40 20 10 5 16 8 4 2 1

Input8:
13
Output8:
13 40 20 10 5 16 8 4 2 1

Input9:
8
Output9:
8 4 2 1

Input10:
7
Output10:
7 22 11 34 17 52 26 13 40 20 10 5 16 8 4 2 1

Templet:
========
import java.util.Scanner;

class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int no = sc.nextInt();
		System.out.println(getCollatzSequence(no));
	}

	public static String getCollatzSequence(int n) {
		//write the code here..
		 
	}
}

Solution:
=========
import java.util.Scanner;

class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int no = sc.nextInt();
		System.out.println(getCollatzSequence(no));
	}

	static String getCollatzSequence(int n) {

		String str = "";
		if (n <= 0) {
			return "Error";
		}
		str = "" + n + " ";

		while (n > 1) {

			if (n % 2 == 0) {
				n = n / 2;
			} else {
				n = (n * 3) + 1;
			}

			str = str + n + " ";

		}
		return str.trim();
	}
}
=====================================================================================================
Program   : FOP_28
Language: Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements & String
Problem Statement:   


For a given method write the logic which returns "FIZZ" if the input is a multiple of 3, prints "BIZZ" if the input is a multiple of 5 and prints "FIZZBIZZ" if the input is a multiple of 3 and 5. 
Print the given input if it is multiple of neither 3 nor 5. 


Specifications: The value returned by the method getFizzBizz() is determined by the following rules:

If the input is a multiple of 3 return "FIZZ" (Ex:- Input 33 output FIZZ)
If the input is a multiple of 5 return "BIZZ" (Ex:- Input 5 output BIZZ)
If the input is a multiple of 3 and 5 return "FIZZBIZZ" (Ex:- Input 15 output FIZZBIZZ)
if the input is not a multiple of 3 or 5, return the number itself in the form of string
If the given value is negative or zero, return "Error"

Constraints
1<=N<10^3

Sample Input1:
3
Sample Output1:
FIZZ

Sample Input2:
5
Sample Output2:
BIZZ

Sample Input3:
-15
Sample Output3:
Error

Sample Input4:
27
Sample Output4:
FIZZ

Sample Input5:
25
Sample Output5:
BIZZ

Sample Input6:
113
Sample Output6:
113

Sample Input7:
225
Sample Output7:
FIZZBIZZ

Sample Input8:
199
Sample Output8:
199

Sample Input9:
999
Sample Output9:
FIZZ

Sample Input10:
8
Sample Output10:
8

Templet:
========
import java.util.Scanner;

public class Test {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(getFizzBizz(num));
	}

	public static String getFizzBizz(int number) {
		//write the code here...
	}
}

Solution:
========
import java.util.Scanner;

public class Test {
	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		System.out.println(getFizzBizz(num));
	}

	public static String getFizzBizz(int number) {
		if (number <= 0)
			return "Error";
		if (number % 3 == 0 && number % 5 == 0)
			return "FIZZBIZZ";
		if (number % 5 == 0)
			return "BIZZ";
		if (number % 3 == 0)
			return "FIZZ";
		return number + "";
	}
}
==========================================================================================================================================
Program   : FOP_29
Language: Java
Level   	   :  Hard
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   


Write the program which accepts an integer value, and check the given number is an perfect, abundant or deficient number.

Explanation:
A number is called perfect:
If the sum of its proper divisors is equal to the number. 
If the sum is less, it is called a deficient number.
If the sum is more than the number, it is called  an abundant number.

Example:
The proper divisors of 28 are 1, 2, 4, 7, 14. 
The sum of those factors 1 + 2 + 4 + 7 + 14 is 28, 
which equal to the number. Hence it is called a perfect number.
Similarly if the sum is less than the number, it is called a deficent number. 
If the sum is greater than the number, it is called an abundant number.
If sum returns -2 then display Error.

Note:
A number is not a proper divisor of itself. Proper divisors of 6 are 1, 2 and 3 only.



Specifications: The value returned by the method sumOfProperDivisors() is determined by the following rules:
If the given number is negative or zero, return -2.
If the sum of proper divisors is equal to the given number, return 0.
If the sum of proper divisors is more than the given number, return 1.
If the sum of proper divisors is less than the given number, return -1.


Constraints:
1<=N<=10^3


Sample Input1:
6
Sample Output1:
Perfect Number

Sample Input2:
10
Sample Output2:
Deficient Number

Sample Input3:
100
Sample Output3:
Abundant Number

Input4:
-12
Output4:
Error

Input5:
0
Output5:
Error

Input6:
122
Output6:
Deficient Number

Input7:
156
Output7:
Abundant Number

Input8:
1
Output8:
Perfect Number

Input9:
999
Output9:
Deficient Number

Input10:
200
Output10:
Abundant Number

Templet:
========
import java.util.Scanner;

public class Test {
	public static void main(String[] args) {
		Scanner sc =new Scanner(System.in);
		int num = sc.nextInt();
		int res = sumOfProperDivisors(num);
		if (res == 0)
			System.out.println("Perfect Number");
		else if (res == 1)
			System.out.println("Abundant Number");
		else if (res == -1)
			System.out.println("Deficient Number");
		else
			System.out.println("Error");
	}

	public static int sumOfProperDivisors(int num) {
		 	//write the code here.....
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {
	public static void main(String[] args) {
		Scanner sc =new Scanner(System.in);
		int num = sc.nextInt();
		int res = sumOfProperDivisors(num);
		if (res == 0)
			System.out.println("Perfect Number");
		else if (res == 1)
			System.out.println("Abundant Number");
		else if (res == -1)
			System.out.println("Deficient Number");
		else
			System.out.println("Error");
	}

	public static int sumOfProperDivisors(int num) {
		if (num <=0)
			return -2;
		
		int sum = 1;
		for (int i = 2; i <= num / 2; i++) {
			if (num % i == 0)
				sum += i;
		}
		if (sum == num)
			return 0;
		if (sum > num)
			return 1;
		return -1;
	}
}
==========================================================================================================================
Program   : FOP_30
Language: Java
Level   	   :  Basic
Module   : Fundamental of Programming
Topic        : Control Statements 
Problem Statement:   

For a given method write a logic to count no of digits of given long number.

Specification: Specifications: The value returned by the method countDigits() is determined by the following rules:
If a number is negative or zero , return -1.
Otherwise return count no of digits of a given number.
 

Sample Input1:
10
Sample Output1:
2

Sample Input2:
-12
Sample Output2:
-1

Sample Input3:
0
Sample Output3:
-1

Input4:
120
Output4:
3

Input5:
1221
Output5:
4

Input6:
10000
Output6:
5

Input7:
321003111
Output7:
9

Input8:
989982712211
Output8:
12

Input9:
223315
Output9:
6

Input10:
9988766
Output10:
7

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		long num = sc.nextLong();
		System.out.println(countDigits(num));
	}

	public static int countDigits(long no) {
		  //write the code here...
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		long num = sc.nextLong();
		System.out.println(countDigits(num));
	}

	public static int countDigits(long no) {
		int count = 0;
		if (no <= 0)
			return -1;
		else if (no >= 1 && no <= 9)
			return -2;
		else {
			while (no != 0) {
				no = no / 10;
				count++;
			}
		}
		return count;
	}
}
==================================================================================================================================================================
					    Pattern Programs
==================================================================================================================================================================
Program   : FOP_31
Language: Java
Level   	   :  Basic
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   

For a given method print star pattern or rectangle star pattern.

Constraints:
2<=N<=10 
Specification : The method starPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print the star pattern.

Sample Input1:
5
Sample Output1:
*****
*****
*****
*****
*****

Sample Input2:
0
Sample Output2:
-1

Sample Input3:
-6
Sample Output3:
-1

Input4:
6
Output4:
******
******
******
******
******
******

Input5:
3
Output5:
***
***
***
Input6:
7
Output6:
*******
*******
*******
*******
*******
*******
*******
Input7:
4
Output7:
****
****
****
****
Input8:
8
Output8:
********
********
********
********
********
********
********
********
Input9:
9
Output9:
*********
*********
*********
*********
*********
*********
*********
*********
*********
Input10:
10
Output10:
**********
**********
**********
**********
**********
**********
**********
**********
**********
**********

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		starPattern(num);
	}

	public static void starPattern(int num) {
			//write the code here...		 
	}

}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		starPattern(num);
	}

	public static void starPattern(int num) {

		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 2 && num <= 10) {
			for (int i = 1; i <= num; i++) {
				for (int j = 1; j <= num; j++) {
					System.out.print("*");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
====================================================================================================
Program   : FOP_32
Language: Java
Level   	   :  Basic
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   
  
For a given method print star pattern  with given no of rows and columns.
Input Format: First line contain ROWS , COLUMNS as integer.
Output Format: Print star pattern , based on rows and columns.

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10;
 
Specification : The method starPattern() is determined by the following rules: 
-If Rows , Columns is negative or zero then print -1.
-If Rows, Columns is not in a range of above constraints then, print -2.
-Otherwise print the star pattern.

Sample Input1:
5 3
Sample Output1:
***
***
***
***
***
Sample Input2:
10 11
Sample Output2:
-2
Sample Input3:
-2 -2 
Sample Output3:
-1

Input4:
4 9
Output4:
*********
*********
*********
*********

Input5:
3 8
Output5:
********
********
********
Input6:
6 6
Output6:
******
******
******
******
******
******

Input7:
8 3
Output7:
***
***
***
***
***
***
***
***
Input8:
10 5
Output8:
*****
*****
*****
*****
*****
*****
*****
*****
*****
*****
Input9:
2 9
Output9:
*********
*********

Input10:
5 10
Output10:
**********
**********
**********
**********
**********

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		starPattern(rows,cols);
	}

	public static void starPattern(int rows,int cols) {
		  //write the code here...		 
	}

}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		starPattern(rows,cols);
	}

	public static void starPattern(int rows,int cols) {

		if (rows <= 0 || cols<=0) {
			System.out.println(-1);
		} else if ((rows >= 2 && rows<= 10) && (cols>=2 && cols<=10)) {
			for (int i = 1; i <= rows; i++) {
				for (int j = 1; j <= cols; j++) {
					System.out.print("*");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
================================================================================================================================
Program   : FOP_33
Language: Java
Level   	   :  Basic
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   


For a given method write a logic to print mirrored rhombus star pattern.
Input Format: First line contain integer.
Output Format: Print mirrored rhombus star pattern.

Constraints:
2<=N<=10;
 
Specification : The method rhombusStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print mirrored rhombus star pattern.

Sample Input1:
5
Sample Output1:
*****
 *****
  *****
   *****
    *****

Sample Input2:
-6
Sample Output2:
-1
Sample Input3:
0
Sample Output3:
-1
Input4:
3
Output4:
***
 ***
  ***
Input5:
4
Output5:
****
 ****
  ****
   ****
Input6:
6
Output6:
******
 ******
  ******
   ******
    ******
     ******
Input7:
7
Output7:
*******
 *******
  *******
   *******
    *******
     *******
      *******

Input8:
10
Output8:
**********
 **********
  **********
   **********
    **********
     **********
      **********
       **********
        **********
         **********
Input9:
9
Output9:
*********
 *********
  *********
   *********
    *********
     *********
      *********
       *********
        *********
        
Input10:
2
Output10:
**
 **

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		rhombusStarPattern(num);
	}

	public static void rhombusStarPattern(int num) {
			//write the code here...	 
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		rhombusStarPattern(num);
	}

	public static void rhombusStarPattern(int num) {

		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 2 && num <= 10) {
			for (int i = 1; i <= num; i++) {
				for (int j = 1; j < i; j++) {
					System.out.print(" ");
				}
				for (int j = 1; j <= num; j++) {
					System.out.print("*");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
====================================================================================================================
Program   : FOP_34
Language: Java
Level   	   :  Basic
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   



 For a given method write  a logic to print mirrored parallelogram star pattern.
Input Format: First line contain ROWS , COLUMNS as integer.
Output Format: Print mirrored parallelogram star pattern , based on rows and columns.

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10;
 
Specification : The method parallelogramStarPattern() is determined by the following rules: 
-If Rows , Columns is negative or zero then print -1.
-If Rows, Columns  is not in a range of above constraints then, print -2.
-Otherwise print the parallelogram star pattern.

Sample Input1:
3 5
Sample Output1:
*****
 *****
  *****
Sample Input2:
0 0
Sample Output2:
-1
Sample Input3:
5 -2
Sample Output3:
-1
Input4:
3 7
Output4:
*******
 *******
  *******
Input5:
7 3
Output5:
***
 ***
  ***
   ***
    ***
     ***
      ***
Input6:
6 8
Output6:
********
 ********
  ********
   ********
    ********
     ********
Input7:
2 5
Output7:
*****
 *****
Input8:
4 2
Output8:
**
 **
  **
   **
Input9:
1 9
Output9:
-2
Input10:
7 1
Output10:
-2

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		rhombusStarPattern(rows,cols);
	}

	public static void rhombusStarPattern(int rows,int cols) {
 			//write the code here...
	}

}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		rhombusStarPattern(rows,cols);
	}

	public static void rhombusStarPattern(int rows,int cols) {

		if (rows <= 0 || cols<=0) {
			System.out.println(-1);
		} else if ((rows >= 2 && rows<= 10) && (cols>=2 && cols<=10)) {
			for (int i = 1; i <= rows; i++) {
				for (int j = 1; j < i; j++) {
					System.out.print(" ");
				}
				for (int j = 1; j <= cols; j++) {
					System.out.print("*");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
=====================================================================================================================================
Program   : FOP_35
Language: Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   
 

For a given method write a logic to print hollow square.

Input Format  : Take N as input of type integer.
Output Format : Print hollow square.


Constraints:
2<=N<=10

Specifation: The method hollowSquarePattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print hollow square pattern.


Sample Input1:
5
Sample Output1:
*****
*   *
*   *
*   *
*****

Sample Input2:
-10
Sample Output2:
-1

Sample Input3:
12
Sample Output3:
-2

Input4:
3
Output4:
***
* *
***
Input5:
6
Output5:
******
*    *
*    *
*    *
*    *
******
Input6:
7
Output6:
*******
*     *
*     *
*     *
*     *
*     *
*******
Input7:
2
Output7:
**
**
Input8:
8
Output8:
********
*      *
*      *
*      *
*      *
*      *
*      *
********

Input9:
4
Output9:
****
*  *
*  *
****
Input10:
9
Output10:
*********
*       *
*       *
*       *
*       *
*       *
*       *
*       *
*********

Templet:
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowSquarePattern(num);
	}

	public static void hollowSquarePattern(int num) {
			//write the code here...	 
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowSquarePattern(num);
	}

	public static void hollowSquarePattern(int num) {

		if (num <= 0)
			System.out.println(-1);
		else if (num >= 2 && num <= 10) {
			for (int i = 1; i <= num; i++) {
				for (int j = 1; j <= num; j++) {
					if (i == 1 || i == num || j == 1 || j == num) {
						System.out.print("*");
					} else {
						System.out.print(" ");
					}
				}

				System.out.println();
			}

		} else {
			System.out.println(-2);
		}
	}

}
============================================================================================================================================
Program   : FOP_36
Language: Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   
 
For a given method write a logic to print  hollow rectangle pattern in a MxN matrix.

Input Format  : Read two integers i.e. M(Rows) and N(Columns).

Output Format : Print the hollow rectangle pattern in a MxN matrix

Constraints:
2<=M<=10
2<=N<=10

Specification : The method hollowRectangleStarPattern() is determined by the following rules: 
-If M ,N is negative or zero then print -1.
-If M, N is not in a range of above constraints then, print -2.
-Otherwise print the hollow rectangle star pattern.

Sample Input1:
5 4
Sample Output1:
****
*  *
*  *
*  *
****
Sample Input2:
5 -3
Sample Output2:
-1
Sample Input3:
10 12
Sample Output3:
-2

Input4:
3 8
Output4:
********
*      *
********
Input5:
4 4
Output5:
****
*  *
*  *
****
Input6:
6 4
Output6:
****
*  *
*  *
*  *
*  *
****
Input7:
7 3
Output7:
***
* *
* *
* *
* *
* *
***
Input8:
6 9
Output8:
*********
*       *
*       *
*       *
*       *
*********
Input9:
2 6
Output9:
******
******
Input10:
9 10
Output10:
**********
*        *
*        *
*        *
*        *
*        *
*        *
*        *
**********

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int M = sc.nextInt();
		int N = sc.nextInt();
		hollowRectangleStarPattern(M, N);
	}

	public static void hollowRectangleStarPattern(int M, int N) {
		 //write the code here.
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int M = sc.nextInt();
		int N = sc.nextInt();
		hollowRectangleStarPattern(M, N);
	}

	public static void hollowRectangleStarPattern(int M, int N) {
		if (M <= 0 || N <= 0)
			System.out.println(-1);
		else if ((M >= 2 && N <= 10) && (N >= 2 && N <= 10)) {
			for (int i = 1; i <= M; i++) {
				for (int j = 1; j <= N; j++) {
					if (i == 1 || i == M || j == 1 || j == N) {
						System.out.print("*");
					} else {
						System.out.print(" ");
					}
				}

				System.out.println();
			}

		} else {
			System.out.println(-2);
		}
	}

}
=======================================================================================================================================
Program   : FOP_37
Language: Java
Level   	   :  Hard
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   

For a given method write a logic to print hollow square star pattern with diagonal.

Input Format  : Take N as input of type integer.

Output Format : Print hollow square star pattern with diagonal.

Constraints:
5<=N<=15

Specification: The method hollowSquareWithDiagonal() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print hollow square star pattern with diagonal.


Sample Input1:
5
Sample Output1:
*****
** **
* * *
** **
*****
Sample Input2:
-6
Sample Output2:
-1
Sample Input3:
21
Sample Output3:
-2

Input4:
7
Output4:
*******
**   **
* * * *
*  *  *
* * * *
**   **
*******
Input5:
6
Output5:
******
**  **
* ** *
* ** *
**  **
******
Input6:
8
Output6:
********
**    **
* *  * *
*  **  *
*  **  *
* *  * *
**    **
********
Input7:
10
Output7:
**********
**      **
* *    * *
*  *  *  *
*   **   *
*   **   *
*  *  *  *
* *    * *
**      **
**********
Input8:
14
Output8:
**************
**          **
* *        * *
*  *      *  *
*   *    *   *
*    *  *    *
*     **     *
*     **     *
*    *  *    *
*   *    *   *
*  *      *  *
* *        * *
**          **
**************

Input9:
12
Output9:
************
**        **
* *      * *
*  *    *  *
*   *  *   *
*    **    *
*    **    *
*   *  *   *
*  *    *  *
* *      * *
**        **
************

Input10:
2
Output10:
-2

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowSquareWithDiagonal(num);
	}
	
	public static void hollowSquareWithDiagonal(int num){
		   //write the code here...
	}

}
Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowSquareWithDiagonal(num);
	}
	
	public static void hollowSquareWithDiagonal(int num){
		   if(num<=0){
			   System.out.println(-1);
		   }else if(num>=5 && num<=15){
			   for(int i=1;i<=num;i++){
				   for(int j=1;j<=num;j++){
					   if(i==1 || i==num || j==1 || j==num || i==j || j==(num-i+1)){
						   System.out.print("*");
					   }else{
						   System.out.print(" ");
					   }
				   }
				   System.out.println();
			   }
		   }else{
			   System.out.println(-2);
		   }
		
		
	}

}
==============================================================================================================================================

Program   : FOP_38
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   



For a given method  write a logic to print hollow rhombus, parallelogram star pattern.

Input Format  : Take N as input of type integer.
Output Format : Print hollow rhombus, parallelogram star pattern.


Constraints:
2<=N<=10

Specifation: The method hollowRhombusParallelogramPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print hollow rhombus, parallelogram star pattern.

Sample Input1:
5
Sample Output1:
    *****
   *   *
  *   *
 *   *
*****
Sample Input2:
-7
Sample Output2:
-1

Sample Input3:
12
Sample Output3:
-2

Input4:
3
Output4:
  ***
 * *
***
Input5:
6
Output5:
     ******
    *    *
   *    *
  *    *
 *    *
******
Input6:
7
Output6:
      *******
     *     *
    *     *
   *     *
  *     *
 *     *
*******
Input7:
2
Output7:
 **
**
Input8:
1
Output8:
-2
Input9:
4
Output9:
   ****
  *  *
 *  *
****

Input10:
10
Output10:
         **********
        *        *
       *        *
      *        *
     *        *
    *        *
   *        *
  *        *
 *        *
**********

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowRhombusParallelogramPattern(num);
	}

	public static void hollowRhombusParallelogramPattern(int num) {
			//write the code here...

	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowRhombusParallelogramPattern(num);
	}

	public static void hollowRhombusParallelogramPattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 2 && num <= 10) {
			for (int i = 1; i <= num; i++) {
				for (int space = 1; space <= num - i; space++) {
					System.out.print(" ");
				}
				for (int j = 1; j <= num; j++) {
					if (i == 1 || i == num || j == 1 || j == num)
						System.out.print("*");
					else
						System.out.print(" ");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}

	}

}
=========================================================================================================================================

Program   : FOP_39
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   

For a given method write the logic to print right triangle star pattern.

Input Format  : Take N as input of type integer.
Output Format : Print the right triangle star pattern.

Constraints:
2<=N<=10

Specification: The method rightTriangleStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print right triangle star pattern.

Sample Input1:
5
Sample Output1:
*
**
***
****
*****
Sample Input2:
-3
Sample Output2:
-1
Sample Input3:
20
Sample Output3:
-2
Input4:
3
Output4:
*
**
***
Input5:
4
Output5:
*
**
***
****
Input6:
6
Output6:
*
**
***
****
*****
******
Input7:
8
Output7:
*
**
***
****
*****
******
*******
********
Input8:
9
Output8:
*
**
***
****
*****
******
*******
********
*********
Input9:
100
Output9:
-2
Input10:
2
Output10:
*
**
Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		rightTriangleStarPattern(num); 
	}
    public static void rightTriangleStarPattern(int num){
			//write the code here...
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		rightTriangleStarPattern(num); 
	}
    public static void rightTriangleStarPattern(int num){
    		if(num<=0){
    			System.out.println(-1);
    		}else if(num>=2 && num<=10){
    			for(int i=1;i<=num;i++){
    				for(int j=1;j<=i;j++){
    					System.out.print("*");
    				}
    				System.out.println();
    			}
    		}else {
    			System.out.println(-2);
    		}
    }
	 
}
================================================================================================================================
Program   : FOP_40
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   


For a given method write the logic to print hollow right triangle star pattern.

Input Format  : Take N as input of type integer.
Output Format : Print hollow right triangle star pattern.

Constraints:
2<=N<=10

Specification: The method hollowRightTriangleStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print hollow right triangle star pattern.

Sample Input1:
5
Sample Output1:
*
**
* *
*  *
*****
Sample Input2:
16
Sample Output2:
-2
Sample Input3:
-4
Sample Output3:
-1
Input4:
2
Output4:
*
**
Input5:
3
Output5:
*
**
***
Input6:
4
Output6:
*
**
* *
****
Input7:
6
Output7:
*
**
* *
*  *
*   *
******
Input8:
7
Output8:
*
**
* *
*  *
*   *
*    *
*******
Input9:
8
Output9:
*
**
* *
*  *
*   *
*    *
*     *
********
Input10:
9
Output10:
*
**
* *
*  *
*   *
*    *
*     *
*      *
*********

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowRightTriangleStarPattern(num); 
	}
    public static void hollowRightTriangleStarPattern(int num){
    		 //write the code here....
    }
	 
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowRightTriangleStarPattern(num); 
	}
    public static void hollowRightTriangleStarPattern(int num){
    		if(num<=0){
    			System.out.println(-1);
    		}else if(num>=2 && num<=10){
    			for(int i=1;i<=num;i++){
    				for(int j=1;j<=i;j++){
    					if(j==1 ||j==i||i==num)
    					System.out.print("*");
    					else
    					System.out.print(" ");
    				}
    				System.out.println();
    			}
    		}else {
    			System.out.println(-2);
    		}
    }
	 
}
=================================================================================================================
Program   : FOP_41
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   

For a given method write the logic to print hollow mirrored right triangle star pattern.

Input Format  : Take N as input of type integer.
Output Format : Print hollow mirrored right triangle star pattern.

Constraints:
2<=N<=10

Specification: The method hollowmirroredRightTrianglePattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print hollow mirrored right triangle star pattern.


Sample Input1:
5
Sample Output1:
    *
   **
  * *
 *  *
*****
Sample Input2:
-7
Sample Output2:
-1
Sample Input3:
13
Sample Output3:
-2
Input4:
3
Output4:
  *
 **
***
Input5:
6
Output5:
     *
    **
   * *
  *  *
 *   *
******
Input6:
7
Output6:
      *
     **
    * *
   *  *
  *   *
 *    *
*******
Input7:
9
Output7:
        *
       **
      * *
     *  *
    *   *
   *    *
  *     *
 *      *
*********
Input8:
2
Output8:
 *
**
Input9:
10
Output9:
         *
        **
       * *
      *  *
     *   *
    *    *
   *     *
  *      *
 *       *
**********
Input10:
4
Output10:
   *
  **
 * *
****

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowRightTriangleStarPattern(num); 
	}
    public static void hollowRightTriangleStarPattern(int num){
    		//write the code here...		 
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowRightTriangleStarPattern(num); 
	}
    public static void hollowRightTriangleStarPattern(int num){
    		if(num<=0){
    			System.out.println(-1);
    		}else if(num>=2 && num<=10){
    			for(int i=1;i<=num;i++){
    				 for(int j=i;j<num;j++){
    					 System.out.print(" ");
    				 }
    				for(int j=1;j<=i;j++){
    					if(j==1 ||j==i||i==num)
    					System.out.print("*");
    					else
    					System.out.print(" ");
    				}
    				System.out.println();
    			}
    		}else {
    			System.out.println(-2);
    		}
    }
	 
}
=================================================================================================================================================
Program   : FOP_42
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   


For a given method write the logic to print mirrored right triangle star pattern.

Input Format  : Take N as input of type integer.
Output Format : Print the mirrored right triangle star pattern.

Constraints:
2<=N<=10

Specification: The method mirroredRightTriangleStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print  mirrored right triangle star pattern.

Sample Input1:
5
Sample Output1:
    *
   **
  ***
 ****
*****
Sample Input2:
1
Sample Output2:
-2
Sample Input3:
-10
Sample Output3:
-1
Input4:
2
Output4:
 *
**
Input5:
3
Output5:
  *
 **
***
Input6:
4
Output6:
   *
  **
 ***
****
Input7:
6
Output7:
     *
    **
   ***
  ****
 *****
******
Input8:
7
Output8:
      *
     **
    ***
   ****
  *****
 ******
*******
Input9:
8
Output9:
       *
      **
     ***
    ****
   *****
  ******
 *******
********
Input10:
9
Output10:
        *
       **
      ***
     ****
    *****
   ******
  *******
 ********
*********

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		mirroredRightTriangleStarPattern(num); 
	}
    public static void mirroredRightTriangleStarPattern(int num){
    		 //write the code here....
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		mirroredRightTriangleStarPattern(num); 
	}
    public static void mirroredRightTriangleStarPattern(int num){
    		if(num<=0){
    			System.out.println(-1);
    		}else if(num>=2 && num<=10){
    			for(int i=1;i<=num;i++){
    				for(int space=i;space<num;space++){
    					System.out.print(" ");
    				}
    				for(int j=1;j<=i;j++){
    					System.out.print("*");
    				}
    				System.out.println();
    			}
    		}else {
    			System.out.println(-2);
    		}
    }
	 
}
=============================================================================================================================================
Program   : FOP_43
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   
 

For a given method write the logic to print reverse right triangle star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print the  reverse right triangle star pattern.

Constraints:
2<=N<=10

Specification: The method reverseRightTriangleStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print reverse right triangle star pattern.

Sample Input1:
5
Sample Output1:
*****
****
***
**
*
Sample Input2:
1
Sample Output2:
-2
Sample Input3:
0
Sample Output3:
-1
Input4:
3
Output4:
***
**
*
Input5:
4
Output5:
****
***
**
*
Input6:
6
Output6:
******
*****
****
***
**
*
Input7:
7
Output7:
*******
******
*****
****
***
**
*
Input8:
8
Output8:
********
*******
******
*****
****
***
**
*
Input9:
9
Output9:
*********
********
*******
******
*****
****
***
**
*
Input10:
10
Output10:
**********
*********
********
*******
******
*****
****
***
**
*

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		reverseRightTriangleStarPattern(num); 
	}
    public static void reverseRightTriangleStarPattern(int num){
    		 //write the code here..
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		reverseRightTriangleStarPattern(num); 
	}
    public static void reverseRightTriangleStarPattern(int num){
    		if(num<=0){
    			System.out.println(-1);
    		}else if(num>=2 && num<=10){
    			 for(int i=1;i<=num;i++){
    				 for(int j=i;j<=num;j++){
    					 System.out.print("*");
    				 }
    				 System.out.println();
    			 }
    		}else {
    			System.out.println(-2);
    		}
    }
	 
}
=============================================================================================================================================
Program   : FOP_44
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   
 

For a given method write the logic to print reversed mirrored right triangle star pattern.

Input Format  : Take N as input of type integer.
Output Format : Print the  reversed mirrored right triangle star pattern.

Constraints:
2<=N<=10

Specification: The method reversedMirroredRightTriangleStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print reversed mirrored right triangle star pattern.

Sample Input1:
5
Sample Output1:
*****
 ****
  ***
   **
    *
Sample Input2:
11
Sample Output2:
-2
Sample Input3:
0
Sample Output3:
-1
Input4:
2
Output4:
**
 *
Input5:
3
Output5:
***
 **
  *
Input6:
4
Output6:
****
 ***
  **
   *
Input7:
6
Output7:
******
 *****
  ****
   ***
    **
     *
Input8:
7
Output8:
*******
 ******
  *****
   ****
    ***
     **
      *
Input9:
8
Output9:
********
 *******
  ******
   *****
    ****
     ***
      **
       *
Input10:
9
Output10:
*********
 ********
  *******
   ******
    *****
     ****
      ***
       **
        *


Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		reversedMirroredRightTriangleStarPattern(num); 
	}
    public static void reversedMirroredRightTriangleStarPattern(int num){
    		 //write the code here...
    }
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		reversedMirroredRightTriangleStarPattern(num); 
	}
    public static void reversedMirroredRightTriangleStarPattern(int num){
    		if(num<=0){
    			System.out.println(-1);
    		}else if(num>=2 && num<=10){
    			 for(int i=1;i<=num;i++){
    				  for(int space=1;space<i;space++){
    					  System.out.print(" ");
    				  }
    				 for(int j=i;j<=num;j++){
    					 System.out.print("*");
    				 }
    				 System.out.println();
    			 }
    		}else {
    			System.out.println(-2);
    		}
    }
	 
}
=========================================================================================================================================================================
Program   : FOP_45
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   



For a given method write the logic to print hollow inverted right triangle star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print hollow inverted right triangle star pattern

Constraints:
5<=N<=15

Specification: The method hollowInvertedRightTrianglePattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print hollow inverted right triangle star pattern.

Sample Input1:
5
Sample Output1:
*****
*  *
* *
**
*
Sample Input2:
21
Sample Output2:
-2
Sample Input3:
-9
Sample Output3:
-1
 
Input4:
6
Output4:
******
*   *
*  *
* *
**
*
Input5:
7
Output5:
*******
*    *
*   *
*  *
* *
**
*
Input6:
8
Output6:
********
*     *
*    *
*   *
*  *
* *
**
*
Input7:
9
Output7:
*********
*      *
*     *
*    *
*   *
*  *
* *
**
*
Input8:
10
Output8:
**********
*       *
*      *
*     *
*    *
*   *
*  *
* *
**
*
Input9:
11
Output9:
***********
*        *
*       *
*      *
*     *
*    *
*   *
*  *
* *
**
*
Input10:
14
Output10:
**************
*           *
*          *
*         *
*        *
*       *
*      *
*     *
*    *
*   *
*  *
* *
**
*

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowInvertedRightTrianglePattern(num);
	}

	public static void hollowInvertedRightTrianglePattern(int num) {
		 		//write the code here...
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowInvertedRightTrianglePattern(num);
	}

	public static void hollowInvertedRightTrianglePattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i <= num; i++) {
				for (int j = i; j <= num; j++) {
					if (i== 1 || j == i || j== num)
						System.out.print("*");
					else
						System.out.print(" ");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
==============================================================================================================================================================

Program   : FOP_46
Language : Java
Level   	   :  Medium
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   

For a given method write the logic to print hollow mirrored inverted right triangle star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print hollow mirrored inverted right triangle star pattern.


Constraints:
5<=N<=15

Specification: The method hollowMirroredInvertedRightTrianglePattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise  to print hollow mirrored inverted right triangle star pattern.

Sample Input1:
5
Sample Output1:
*****
 *  *
  * *
   **
    *
Sample Input2:
2
Sample Output2:
-2
Sample Input3:
0
Sample Output3:
-1
Input4:
6
Output4:
******
 *   *
  *  *
   * *
    **
     *
Input5:
7
Output5:
*******
 *    *
  *   *
   *  *
    * *
     **
      *
Input6:
8
Output6:
********
 *     *
  *    *
   *   *
    *  *
     * *
      **
       *
Input7:
10
Output7:
**********
 *       *
  *      *
   *     *
    *    *
     *   *
      *  *
       * *
        **
         *
Input8:
11
Output8:
***********
 *        *
  *       *
   *      *
    *     *
     *    *
      *   *
       *  *
        * *
         **
          *
Input9:
12
Output9:
************
 *         *
  *        *
   *       *
    *      *
     *     *
      *    *
       *   *
        *  *
         * *
          **
           *
Input10:
-15
Output10:
-1

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowMirroredInvertedRightTrianglePattern(num);
	}

	public static void hollowMirroredInvertedRightTrianglePattern(int num) {
		 //write the code here...
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowMirroredInvertedRightTrianglePattern(num);
	}

	public static void hollowMirroredInvertedRightTrianglePattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i <= num; i++) {
				  for(int space=1;space<i;space++){
					  System.out.print(" ");
				  }
				for (int j = i; j <= num; j++) {
					if (i== 1 || j == i || j== num)
						System.out.print("*");
					else
						System.out.print(" ");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
===============================================================================================================================================
Program   : FOP_47
Language : Java
Level   	   :  Hard
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement:   

For a given method write the logic to print Equilateral triangle (Pyramid) star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print Equilateral triangle (Pyramid) star pattern.


Constraints:
5<=N<=15

Specification: The method pyramidStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise  to print Equilateral triangle (Pyramid) star pattern.

Sample Input1:
5
Sample Output1:
    *
   ***
  *****
 *******
*********
Sample Input2:
2
Sample Output2:
-2
Sample Input3:
-6
Sample Output3:
-1
Input4:
6
Output4:
     *
    ***
   *****
  *******
 *********
***********
Input5:
7
Output5:
      *
     ***
    *****
   *******
  *********
 ***********
*************
Input6:
8
Output6:
       *
      ***
     *****
    *******
   *********
  ***********
 *************
***************
Input7:
10
Output7:
         *
        ***
       *****
      *******
     *********
    ***********
   *************
  ***************
 *****************
*******************
Input8:
9
Output8:
        *
       ***
      *****
     *******
    *********
   ***********
  *************
 ***************
*****************
Input9:
11
Output9:
          *
         ***
        *****
       *******
      *********
     ***********
    *************
   ***************
  *****************
 *******************
*********************
Input10:
31
Output10:
-2

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		pyramidStarPattern(num);
	}

	public static void pyramidStarPattern(int num) {
		 //write the code here.
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		pyramidStarPattern(num);
	}

	public static void pyramidStarPattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i <= num; i++) {
				  for(int space=i;space<num;space++){
					  System.out.print(" ");
				  }
				for (int j = 1; j <=(2*i-1); j++) {
					System.out.print("*");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
====================================================================================================================================
Program   : FOP_48
Language : Java
Level   	   :  Hard
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
Problem Statement: 
For a given method write the logic to print reverse Pyramid star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print reverse Pyramid star pattern.


Constraints:
5<=N<=15

Specification: The method reversePyramidStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise to print reverse Pyramid star pattern.

Sample Input1:
5
Sample Output1:
*********
 *******
  *****
   ***
    *
Sample Input2:
4
Sample Output2:
-2
Sample Input3:
-7
Sample Output3:
-1
Input4:
6
Output4:
***********
 *********
  *******
   *****
    ***
     *
Input5:
7
Output5:
*************
 ***********
  *********
   *******
    *****
     ***
      *
Input6:
8
Output6:
***************
 *************
  ***********
   *********
    *******
     *****
      ***
       *
Input7:
9
Output7:
*****************
 ***************
  *************
   ***********
    *********
     *******
      *****
       ***
        *
Input8:
11
Output8:
*********************
 *******************
  *****************
   ***************
    *************
     ***********
      *********
       *******
        *****
         ***
          *
Input9:
31
Output9:
-2
Input10:
20
Output10:
-2

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		reversePyramidStarPattern(num);
	}

	public static void reversePyramidStarPattern(int num) {
		  //write the code here...
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		reversePyramidStarPattern(num);
	}

	public static void reversePyramidStarPattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i <=num; i++) {
				  for(int space=1;space<i;space++){
					  System.out.print(" ");
				  }
				for (int j = 1; j <=(num*2-(2*i-1)); j++) {
					System.out.print("*");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
=====================================================================================================================================
Program   : FOP_49
Language : Java
Level   	   :  Hard
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
For a given method write the logic to print hollow pyramid (Equilateral triangle) star pattern.


Input  Format  : Take N as input of type integer.
Output Format  : Print hollow pyramid (Equilateral triangle) star pattern.


Constraints:
5<=N<=15

Specification: The method hollowPyramidStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise  to print hollow pyramid (Equilateral triangle) star pattern.

Sample Input1:
5
Sample Output1:
    *
   * *
  *   *
 *     *
*********
Sample Input2:
3
Sample Output2:
-2
Sample Input3:
-10
Sample Output3:
-1
Input4:
6
Output4:
     *
    * *
   *   *
  *     *
 *       *
***********
Input5:
7
Output5:
      *
     * *
    *   *
   *     *
  *       *
 *         *
*************
Input6:
8
Output6:
       *
      * *
     *   *
    *     *
   *       *
  *         *
 *           *
***************
Input7:
9
Output7:
        *
       * *
      *   *
     *     *
    *       *
   *         *
  *           *
 *             *
*****************
Input8:
19
Output8:
-2
Input9:
11
Output9:
          *
         * *
        *   *
       *     *
      *       *
     *         *
    *           *
   *             *
  *               *
 *                 *
*********************
Input10:
100
Output10:
-2

Templet:
=======

import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowPyramidStarPattern(num);
	}

	public static void hollowPyramidStarPattern(int num) {
				//write the code here...		 
	}

}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowPyramidStarPattern(num);
	}

	public static void hollowPyramidStarPattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i <=num; i++) {
				  for(int space=i;space<num;space++){
					  System.out.print(" ");
				  }
				for (int j = 1; j <=(2*i-1); j++) {
					 if(i==num || j==1 || j==(2*i-1))
					System.out.print("*");
					 else
					System.out.print(" ");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
===========================================================================================================================
Program   : FOP_50
Language : Java
Level   	   :  Hard
Module   : Fundamental of Programming
Topic        : Control Statements 
Subtopic: Star Pattern
For a given method write the logic to print hollow inverted pyramid star pattern.


Input  Format  : Take N as input of type integer.
Output Format  : Print hollow inverted pyramid star pattern.


Constraints:
5<=N<=15

Specification: The method hollowInvertedPyramidStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise  print hollow inverted pyramid star pattern.

Sample Input1:
5
Sample Output1:
*********
 *     *
  *   *
   * *
    *
Sample Input2:
2
Sample Output2:
-2
Sample Input3:
-10
Sample Output3:
-1
Input4:
6
Output4:
***********
 *       *
  *     *
   *   *
    * *
     *
Input5:
7
Output5:
*************
 *         *
  *       *
   *     *
    *   *
     * *
      *
Input6:
8
Output6:
***************
 *           *
  *         *
   *       *
    *     *
     *   *
      * *
       *
Input7:
9
Output7:
*****************
 *             *
  *           *
   *         *
    *       *
     *     *
      *   *
       * *
        *
Input8:
2001
Output8:
-2
Input9:
2343
Output9:
-2
Input10:
-123
Output10:
-1

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowInvertedPyramidStarPattern(num);
	}

	public static void hollowInvertedPyramidStarPattern(int num) {
		   //write the code here...
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		hollowInvertedPyramidStarPattern(num);
	}

	public static void hollowInvertedPyramidStarPattern(int num) {
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i <=num; i++) {
				  for(int space=1;space<i;space++){
					  System.out.print(" ");
				  }
				for (int j = 1; j <=(num*2-(2*i-1)); j++) {
					 if(i==1||j==1||j==(num*2-(2*i-1)))
					System.out.print("*");
					 else
					System.out.print(" ");
				}
				System.out.println();
			}
		} else {
			System.out.println(-2);
		}
	}

}
======================================================================================================================================
						FOP_51 to FOP_100
====================================================================================================================================
Program   : FOP_51
Language  : Java
Level     : Medium
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops
Problem Statement:   
For a given method write the logic to print half diamond star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print half diamond star pattern.

Constraints:
5<=N<=15

Specification: The method halfDiamondStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise  print half diamond star pattern.

Sample Input1:
5
Sample Output1:
*
**
***
****
*****
****
***
**
*
Sample Input2:
-7
Sample Output2:
-1
Sample Input3:
20
Sample Output3:
-2
Input4:
6
Output4:
*
**
***
****
*****
******
*****
****
***
**
*
Input5:
7
Output5:
*
**
***
****
*****
******
*******
******
*****
****
***
**
*
Input6:
8
Output6:
*
**
***
****
*****
******
*******
********
*******
******
*****
****
***
**
Input7:
3
Output7:
-2
Input8:
122331
Output8:
-2
Input9:
-19928
Output9:
-1
Input10:
9
Output10:
*
**
***
****
*****
******
*******
********
*********
********
*******
******
*****
****
***
**
*

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		halfDiamondStarPattern(num);
	}

	public static void halfDiamondStarPattern(int num) {
		 	//write the code here..
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		halfDiamondStarPattern(num);
	}

	public static void halfDiamondStarPattern(int num) {
		int column = 1;
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i < num * 2; i++) {
				for (int j = 1; j <= column; j++) {
					System.out.print("*");
				}
				if (i < num) {
					column++;
				} else {
					column--;
				}
				System.out.println();
			}

		} else {
			System.out.print(-2);
		}
	}
}
==================================================================================================================
Program   : FOP_52
Language  : Java
Level     : Medium
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops
Problem Statement: 

For a given method write the logic to print mirrored half diamond star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print mirrored half diamond star pattern.

Constraints:
5<=N<=15

Specification: The method mirroredHalfDiamondStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print mirrored half diamond star pattern.

Sample Input1:
5
Sample Output1:
    *
   **
  ***
 ****
*****
 ****
  ***
   **
    *
Sample Input2:
3
Sample Output2:
-2
Sample Input3:
-10
Sample Output3:
-1
Input4:
6
Output4:
     *
    **
   ***
  ****
 *****
******
 *****
  ****
   ***
    **
     *
Input5:
7
Output5:
      *
     **
    ***
   ****
  *****
 ******
*******
 ******
  *****
   ****
    ***
     **
      *
Input6:
9990
Output6:
-2
Input7:
-2221
Output7:
-1
Input8:
71
Output8:
-2
Input9:
8
Output9:
       *
      **
     ***
    ****
   *****
  ******
 *******
********
 *******
  ******
   *****
    ****
     ***
      **
       *
Input10:
10
Output10:
         *
        **
       ***
      ****
     *****
    ******
   *******
  ********
 *********
**********
 *********
  ********
   *******
    ******
     *****
      ****
       ***
        **
         *
Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		halfDiamondStarPattern(num);
	}

	public static void halfDiamondStarPattern(int num) {
		 		//write the code here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		halfDiamondStarPattern(num);
	}

	public static void halfDiamondStarPattern(int num) {
		int column = 1;
		int space = num-1;
		 
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i < num * 2; i++) {
				for(int k=1;k<=space;k++){
					System.out.print(" ");
				}
				for (int j = 1; j <= column; j++) {
					System.out.print("*");
				}
				if (i < num) {
					column++;
					space--;
				} else {
					column--;
					space++;
				}
				System.out.println();
			}

		} else {
			System.out.print(-2);
		}
	}
}
==========================================================================================================================
Program   : FOP_53
Language  : Java
Level     : Hard
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops
For a given method write the logic to print diamond star pattern.

Input  Format  : Take N as input of type integer.
Output Format  : Print diamond star pattern.

Constraints:
5<=N<=15

Specification: The method diamondStarPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is not in a range of above constraints then, print -2.
-Otherwise print diamond star pattern.

Sample Input1:
5
Sample Output1:
    *
   ***
  *****
 *******
*********
 *******
  *****
   ***
    *
Sample Input2:
1
Sample Output2:
-2
Sample Input3:
20
Sample Output3:
-2
Input4:
6
Output4:
     *
    ***
   *****
  *******
 *********
***********
 *********
  *******
   *****
    ***
     *
Input5:
7
Output5:
      *
     ***
    *****
   *******
  *********
 ***********
*************
 ***********
  *********
   *******
    *****
     ***
      *
Input6:
999
Output6:
-2
Input7:
-166
Output7:
-1
Input8:
8
Output8:
       *
      ***
     *****
    *******
   *********
  ***********
 *************
***************
 *************
  ***********
   *********
    *******
     *****
      ***
       *
Input9:
11
Output9:
          *
         ***
        *****
       *******
      *********
     ***********
    *************
   ***************
  *****************
 *******************
*********************
 *******************
  *****************
   ***************
    *************
     ***********
      *********
       *******
        *****
         ***
          *
Input10:
100
Output10:
-2

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		diamondStarPattern(num);
	}

	public static void diamondStarPattern(int num) {
		 	//write the code here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int num = sc.nextInt();
		diamondStarPattern(num);
	}

	public static void diamondStarPattern(int num) {
		int column = 1;
		int space = num-1;
		 
		if (num <= 0) {
			System.out.println(-1);
		} else if (num >= 5 && num <= 15) {
			for (int i = 1; i < num * 2; i++) {
				for(int k=1;k<=space;k++){
					System.out.print(" ");
				}
				for (int j = 1; j <column*2; j++) {
					System.out.print("*");
				}
				if (i < num) {
					column++;
					space--;
				} else {
					column--;
					space++;
				}
				System.out.println();
			}

		} else {
			System.out.print(-2);
		}
	}
}
======================================================================================================
Program   : FOP_54
Language  : Java
Level     : Easy
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops

For a given method write the logic to print 0 or 1 square number pattern.

Input  Format  : Input number of rows and columns to print from user. 
Store it in some variable say rows and cols.
Output Format  : Print 0 or 1 square number pattern.

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10
Specification: The method squareNumberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise print 0 or 1 square number pattern..

 
Sample Input1:
5  5
Sample Output1:
11111
11111
11111
11111
11111
Sample Input2:
6 -7
Sample Output2:
-1
Sample Input3:
0 5
Sample Output3:
-1
Input4:
1 10
Output4:
-2
Input5:
6 6 
Output5:
111111
111111
111111
111111
111111
111111
Input6:
6 6 
Output6:
111111
111111
111111
111111
111111
111111
Input7:
5 10
Output7:
1111111111
1111111111
1111111111
1111111111
1111111111
Input8:
6 9
Output8:
111111111
111111111
111111111
111111111
111111111
111111111
Input9:
7 10
Output9:
1111111111
1111111111
1111111111
1111111111
1111111111
1111111111
1111111111
Input10:
6 8
Output10:
11111111
11111111
11111111
11111111
11111111
11111111

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		squareNumberPattern(rows, cols);
	}

	public static void squareNumberPattern(int rows, int cols) {
				//write the code here...		 
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		squareNumberPattern(rows, cols);
	}

	public static void squareNumberPattern(int rows, int cols) {

		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 2 && rows <= 10 && cols >= 2 && cols <= 10) {
			for (int i = 1; i <= rows; i++) {
				for (int j = 1; j <= cols; j++) {
					System.out.print(1);
				}
				System.out.println();
			}

		} else {
			System.out.print(-2);
		}
	}
}
====================================================================================================================
Program   : FOP_55
Language  : Java
Level     : Easy
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops
Problem Statement :
For a given method write the logic to print number pattern with 1, 0 at alternate rows.

Input  Format  : First line contains input numbers i.e. rows and columns. 
				 
Output Format  : Second line Print the number pattern with 1, 0 at alternate rows.

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise print number pattern with 1, 0 at alternate rows.

Sample Input1:
5 5
Sample Output1
11111
00000
11111
00000
11111

Sample Input2:
5 12
Sample Output2:
-2
Sample Input3:
-6 6
Sample Output3:
-1
Input4:
6 8
Output4:
11111111
00000000
11111111
00000000
11111111
00000000
Input5:
6 9
Output5:
111111111
000000000
111111111
000000000
111111111
000000000
Input6:
7 5
Output6:
11111
00000
11111
00000
11111
00000
11111
Input7:
8 5
Output7:
11111
00000
11111
00000
11111
00000
11111
00000
Input8:
9 4
Output8:
1111
0000
1111
0000
1111
0000
1111
0000
1111
Input9:
3 10
Output9:
1111111111
0000000000
1111111111
Input10:
4 7
Output10:
1111111
0000000
1111111
0000000

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
 				//write the code here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {

		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 2 && rows <= 10 && cols >= 2 && cols <= 10) {
			 for(int i=1;i<=rows;i++) {
				 for(int j=1;j<=cols;j++) {
					 if(i%2==1){
						 System.out.print(1);
					 }else{
						 System.out.print(0);
					 }
				 }
				 System.out.println();
			 }
		} else {
			System.out.print(-2);
		}
	}
}
=======================================================================================================================
Program   : FOP_56
Language  : Java
Level     : Easy
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops

For a given method write the logic to print number pattern with 1, 0 at even/odd columns.

Input  Format  : First line contains input numbers i.e. rows and columns. 
				 
Output Format  : Second line print number pattern with 1, 0 at even/odd columns.  

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise print number pattern with 1, 0 at even/odd columns.


Sample Input1:
5 5
Sample Output1:
01010
01010
01010
01010
01010
Sample Input2:
-10 5
Sample Output2:
-1
Sample Input3:
12 13
Sample Output3:
-2
Input4:
6 6
Output4:
010101
010101
010101
010101
010101
010101
Input5:
7 4
Output5:
0101
0101
0101
0101
0101
0101
0101
Input6:
5 8
Output6:
01010101
01010101
01010101
01010101
01010101
Input7:
7 9
Output7:
010101010
010101010
010101010
010101010
010101010
010101010
010101010
Input8:
8 7
Output8:
0101010
0101010
0101010
0101010
0101010
0101010
0101010
0101010
Input9:
5 3
Output9:
010
010
010
010
010
Input10:
8 8
Output10:
01010101
01010101
01010101
01010101
01010101
01010101
01010101
01010101

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
 					//write the code here....
	}
} 

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {

		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 2 && rows <= 10 && cols >= 2 && cols <= 10) {
			 for(int i=1;i<=rows;i++) {
				 for(int j=1;j<=cols;j++) {
					 if(j%2==1){
						 System.out.print(0);
					 }else{
						 System.out.print(1);
					 }
				 }
				 System.out.println();
			 }
		} else {
			System.out.print(-2);
		}
	}
}
================================================================================================================
Program   : FOP_57
Language  : Java
Level     : Easy
Module    : Fundamental of Programming
Topic     : Control Statements 
Subtopic  : Loops
Problem Statement : 
For a given method write the logic to print number pattern at even/odd columns.

Input  Format  : First line contains input numbers i.e. rows and columns. 
				 
Output Format  : Second line to print number pattern at even/odd columns.  

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise  to print number pattern at even/odd columns.

Sample Input1:
5 5
Sample Output1:
10101
10101
10101
10101
10101
Sample Input2:
5 0
Sample Output2:
-1
Sample Input3:
12 21
Sample Output3:
-2
Input4:
6 5
Output4:
10101
10101
10101
10101
10101
10101
Input5:
7 6
Output5:
101010
101010
101010
101010
101010
101010
101010
Input6:
3 8
Output6:
10101010
10101010
10101010
Input7:
9 8
Output7:
10101010
10101010
10101010
10101010
10101010
10101010
10101010
10101010
10101010
Input8:
4 5
Output8:
10101
10101
10101
10101
Input9:
3 3
Output9:
101
101
101
Input10:
8 9
Output10:
101010101
101010101
101010101
101010101
101010101
101010101
101010101
101010101

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
 				//write the code here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {

		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 2 && rows <= 10 && cols >= 2 && cols <= 10) {
			 for(int i=1;i<=rows;i++) {
				 for(int j=1;j<=cols;j++) {
					 if(j%2==0){
						 System.out.print(0);
					 }else{
						 System.out.print(1);
					 }
				 }
				 System.out.println();
			 }
		} else {
			System.out.print(-2);
		}
	}
}
==================================================================================================================
Program   		  : FOP_58
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic to print chessboard number pattern with 1 and 0.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print chessboard number pattern with 1 and 0.  

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise to print chessboard number pattern with 1 and 0.

Sample Input1:
5 5
Sample Output1:
10101
01010
10101
01010
10101
Sample Input2:
12 12
Sample Output2:
-2
Sample Input3:
-6 -6
Sample Output3:
-1
Input4:
6 6
Output4:
101010
010101
101010
010101
101010
010101
Input5:
6 7
Output5:
1010101
0101010
1010101
0101010
1010101
0101010
Input6:
8 8
Output6:
10101010
01010101
10101010
01010101
10101010
01010101
10101010
01010101
Input7:
9 9
Output7:
101010101
010101010
101010101
010101010
101010101
010101010
101010101
010101010
101010101
Input8:
10 10
Output8:
1010101010
0101010101
1010101010
0101010101
1010101010
0101010101
1010101010
0101010101
1010101010
0101010101
Input9:
8 4
Output9:
1010
0101
1010
0101
1010
0101
1010
0101
Input10:
7 7
1010101
0101010
1010101
0101010
1010101
0101010
1010101

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 		//write the logic here...
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
			int pass  =1;
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 2 && rows <= 10 && cols >= 2 && cols <= 10) {
			 for(int i=1;i<=rows;i++) {
				 for(int j=1;j<=cols;j++) {
					 if(pass==1){
						 System.out.print(1);
					 }else{
						 System.out.print(0);
					 }
					 //update the pass
					 pass = pass*-1;
				 }
				 if(cols%2==0){
					 pass = pass*-1;
				 }
				 System.out.println();
			 }
		} else {
			System.out.print(-2);
		}
	}
}
===============================================================================================================
Program   		  : FOP_59
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement :
For a given method write the logic to print box number pattern with 1 and 0.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print box number pattern with 1 and 0.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise to print box number pattern with 1 and 0.

Sample Input1:
5 5
Sample Output1:
11111
10001
10001
10001
11111
Sample Input2:
1 2
Sample Output2:
-2
Sample Input3:
-6 -6
Sample Output3:
-1
Input4:
6 6
Output4:
111111
100001
100001
100001
100001
111111
Input5:
7 7
Output5:
1111111
1000001
1000001
1000001
1000001
1000001
1111111
Input6:
6 8
Output6:
11111111
10000001
10000001
10000001
10000001
11111111
Input7:
6 9
Output7:
111111111
100000001
100000001
100000001
100000001
111111111
Input8:
7 10
Output8:
1111111111
1000000001
1000000001
1000000001
1000000001
1000000001
1111111111
Input9:
9 11
Output9:
11111111111
10000000001
10000000001
10000000001
10000000001
10000000001
10000000001
10000000001
11111111111
Input10:
6 12
Output10:
111111111111
100000000001
100000000001
100000000001
100000000001
111111111111

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
 				//write the code here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {

		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
			for (int i = 1; i <= rows; i++) {
				for (int j = 1; j <= cols; j++) {
					/*
					 * Print 1 if its first or last row Print 1 if its first or
					 * last column
					 */
					if (i == 1 || i == rows || j == 1 || j == cols) {
						System.out.print("1");
					} else {
						System.out.print("0");
					}
				}

				System.out.print("\n");
			}
		} else {
			System.out.println("-2");
		}
	}
}
==========================================================================================================================================
Program   		  : FOP_60
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement :
For a given method write the logic  to print box number pattern of 1 and 0 with cross center.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line  to print box number pattern of 1 and 0 with cross center.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows and columns both are not equal and if Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise  to print box number pattern of 1 and 0 with cross center.


Sample Input1:
5 5
Sample Output1:
10001
01010
00100
01010
10001
Sample Input2:
6 5
Sample Output2:
-2
Sample Intput3:
-5 -5
Sample Output3:
-1
Input4:
6 6
Output4:
100001
010010
001100
001100
010010
100001
Input5:
7 7
Output5:
1000001
0100010
0010100
0001000
0010100
0100010
1000001
Input6:
8 8
Output6:
10000001
01000010
00100100
00011000
00011000
00100100
01000010
10000001
Input7:
9 9
Output7:
100000001
010000010
001000100
000101000
000010000
000101000
001000100
010000010
100000001
Input8:
11 11
Output8:
10000000001
01000000010
00100000100
00010001000
00001010000
00000100000
00001010000
00010001000
00100000100
01000000010
10000000001
Input9:
10 10
Output9:
1000000001
0100000010
0010000100
0001001000
0000110000
0000110000
0001001000
0010000100
0100000010
1000000001
Input10:
12 16
Output10:
-2

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		   //write the code here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows == cols) {
			if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
				for (int i = 1; i <= rows; i++) {
					for (int j = 1; j <= cols; j++) {
						if (i == j || (j == (cols + 1) - i)) {
							System.out.print(1);
						} else {
							System.out.print(0);
						}
					}

					System.out.println();
				}
			}
		} else {
				System.out.println(-2);
		}
	}
}
==================================================================================================================================
Program   		  : FOP_61
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to print circle box number pattern with 1 and 0.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line   to print circle box number pattern with 1 and 0.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise  to print circle box number pattern with 1 and 0.

Sample Input1:
5 5
Sample Output1:
01110
10001
10001
10001
01110
Sample Input2:
6 0
Sample Output2:
-1
Sample Input3:
10 16
Sample Output3:
-2
Input4:
6 7
Output4:
0111110
1000001
1000001
1000001
1000001
0111110
Input5:
7 7
Output5:
0111110
1000001
1000001
1000001
1000001
1000001
0111110
Input6:
8 6
Output6:
011110
100001
100001
100001
100001
100001
100001
011110
Input7:
9 8
Output7:
01111110
10000001
10000001
10000001
10000001
10000001
10000001
10000001
01111110
Input8:
6 10
Output8:
0111111110
1000000001
1000000001
1000000001
1000000001
0111111110
Input9:
7 10
Output9:
0111111110
1000000001
1000000001
1000000001
1000000001
1000000001
0111111110
Input10:
6 12
Output10:
011111111110
100000000001
100000000001
100000000001
100000000001
011111111110

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 		//write the logic here..
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		}else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
				for (int i = 1; i <= rows; i++) {
					for (int j = 1; j <= cols; j++) {
						// Print corner element
						if ((i == 1 || i == rows) && (j == 1 || j == cols)) {
							System.out.print(0);
						} else if (i == 1 || i == rows || j == 1 || j == cols) {
							// Print edge
							System.out.print(1);
						} else {
							// Print center
							System.out.print(0);
						}
					}

					System.out.println();
				}
			
		} else {
			System.out.println(-2);
		}
	}
}
=========================================================================================================================================================
Program   		  : FOP_62
Language 		  : Java
Level    		  : Easy
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to basic number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print basic number pattern.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise to print the basic number pattern.

Sample Input1:
5 5
Sample Output1:
11111
22222
33333
44444
55555
Sample Input2:
6 -6
Sample Output2:
-1
Sample Input3:
12 20
Sample Output3:
-2

Input4:
6 7 
Output4:
1111111
2222222
3333333
4444444
5555555
6666666

Input5:
7 8
Output5:
11111111
22222222
33333333
44444444
55555555
66666666
77777777
Input6:
8 9
Output6:
111111111
222222222
333333333
444444444
555555555
666666666
777777777
888888888

Input7:
9 10
Output7:
1111111111
2222222222
3333333333
4444444444
5555555555
6666666666
7777777777
8888888888
9999999999

Input8:
7 12
Output8:
111111111111
222222222222
333333333333
444444444444
555555555555
666666666666
777777777777
Input9:
9 14
Output9:
11111111111111
22222222222222
33333333333333
44444444444444
55555555555555
66666666666666
77777777777777
88888888888888
99999999999999

Input10:
5 15
Output10:
111111111111111
222222222222222
333333333333333
444444444444444
555555555555555

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 		//write the code here...
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		}else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
				for (int i = 1; i <= rows; i++) {
					for (int j = 1; j <= cols; j++) {
						  System.out.print(i);
					}

					System.out.println();
				}
			
		} else {
			System.out.println(-2);
		}
	}
}
=====================================================================================================================================================================
Program   		  : FOP_63
Language 		  : Java
Level    		  : Easy
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to basic number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print basic number pattern.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise to print the basic number pattern.

Sample Input1:
5 5
Sample Output1:
12345
12345
12345
12345
12345

Sample Input2:
-10 12
Sample Output2:
-1

Sample Input3:
16 17
Sample Output3:
-2

Input4:
6 7
Output4:
1234567
1234567
1234567
1234567
1234567
1234567

Input5:
7 8
Output5:
12345678
12345678
12345678
12345678
12345678
12345678
12345678

Input6:
5 10
Output6:
12345678910
12345678910
12345678910
12345678910
12345678910

Input7:
6 12
Output7:
123456789101112
123456789101112
123456789101112
123456789101112
123456789101112
123456789101112
 
Input8:
7 14
Output8:
1234567891011121314
1234567891011121314
1234567891011121314
1234567891011121314
1234567891011121314
1234567891011121314
1234567891011121314

Input9:
7 7
Output9:
1234567
1234567
1234567
1234567
1234567
1234567
1234567

Input10:
8 6
Output10:
123456
123456
123456
123456
123456
123456
123456
123456

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 		//write the code here...
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		}else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
				for (int i = 1; i <= rows; i++) {
					for (int j = 1; j <= cols; j++) {
						  System.out.print(j);
					}

					System.out.println();
				}
			
		} else {
			System.out.println(-2);
		}
	}
}
==============================================================================================================================
Program   		  : FOP_64
Language 		  : Java
Level    		  : Easy
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to basic number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print basic number pattern.  

Constraints:
2<=ROWS<=10
2<=COLUMNS<=10
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or Columns is not in a range of above constraints then, print -2.
-Otherwise to print the basic number pattern.

Sample Input1:
5 5 
Sample Output1:
12345
23456
34567
45678
56789

Sample Input2:
-4 -5
Sample Output2:
-1

Sample Input3:
11 12
Sample Output3:
-2

Input4:
3 3
Output4:
123
234
345

Input5:
4 4
Output5:
1234
2345
3456
4567

Input6:
6 6
Output6:
123456
234567
345678
456789
5678910
67891011

Input7:
5 6
Output7:
123456
234567
345678
456789
5678910

Input8:
6 8
Output8:
12345678
23456789
345678910
4567891011
56789101112
678910111213

Input9:
7 7
Output9:
1234567
2345678
3456789
45678910
567891011
6789101112
78910111213

Input10:
5 8
Output10:
12345678
23456789
345678910
4567891011
56789101112

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 	//write the code here...
	}
}

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		}else if (rows >= 2 && rows <= 10 && cols >= 2 && cols <= 10) {
				for (int i = 1; i <= rows; i++) {
					for (int j = i; j<cols+i; j++) {
						  System.out.print(j);
					}

					System.out.println();
				}
			
		} else {
			System.out.println(-2);
		}
	}
}
===================================================================================================================================================
Program   		  : FOP_65
Language 		  : Java
Level    		  : Easy
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to basic number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print basic number pattern were each column number gets printed in an incremented fashion.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or  Columns  is not in a range of above constraints then, print -2.
-Otherwise to print basic number pattern were each column number gets printed in an incremented fashion.

Sample Input1:
5 5
Sample Output1:
1  2  3  4  5  
6  7  8  9  10 
11 12 13 14 15 
16 17 18 19 20 
21 22 23 24 25 

Sample Input2:
2 2
Sample Output2:
-2

Sample Input3:
-5 -7
Sample Output3:
-1

Input4:
6 6
Output4:
1  2  3  4  5  6  
7  8  9  10 11 12 
13 14 15 16 17 18 
19 20 21 22 23 24 
25 26 27 28 29 30 
31 32 33 34 35 36 

Input5:
7 5
Output5:
1  2  3  4  5  
6  7  8  9  10 
11 12 13 14 15 
16 17 18 19 20 
21 22 23 24 25 
26 27 28 29 30 
31 32 33 34 35 

Input6:
7 8
Output6:
1  2  3  4  5  6  7  8  
9  10 11 12 13 14 15 16 
17 18 19 20 21 22 23 24 
25 26 27 28 29 30 31 32 
33 34 35 36 37 38 39 40 
41 42 43 44 45 46 47 48 
49 50 51 52 53 54 55 56 

Input7:
8 9
Output7:
1  2  3  4  5  6  7  8  9  
10 11 12 13 14 15 16 17 18 
19 20 21 22 23 24 25 26 27 
28 29 30 31 32 33 34 35 36 
37 38 39 40 41 42 43 44 45 
46 47 48 49 50 51 52 53 54 
55 56 57 58 59 60 61 62 63 
64 65 66 67 68 69 70 71 72 

Input8:
9 10
Output8:
1  2  3  4  5  6  7  8  9  10 
11 12 13 14 15 16 17 18 19 20 
21 22 23 24 25 26 27 28 29 30 
31 32 33 34 35 36 37 38 39 40 
41 42 43 44 45 46 47 48 49 50 
51 52 53 54 55 56 57 58 59 60 
61 62 63 64 65 66 67 68 69 70 
71 72 73 74 75 76 77 78 79 80 
81 82 83 84 85 86 87 88 89 90 

Input9:
6 9
Output9:
1  2  3  4  5  6  7  8  9  
10 11 12 13 14 15 16 17 18 
19 20 21 22 23 24 25 26 27 
28 29 30 31 32 33 34 35 36 
37 38 39 40 41 42 43 44 45 
46 47 48 49 50 51 52 53 54 

Input10:
11 6
Output10:
1  2  3  4  5  6  
7  8  9  10 11 12 
13 14 15 16 17 18 
19 20 21 22 23 24 
25 26 27 28 29 30 
31 32 33 34 35 36 
37 38 39 40 41 42 
43 44 45 46 47 48 
49 50 51 52 53 54 
55 56 57 58 59 60 
61 62 63 64 65 66 

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 	//write the code here..
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		}else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
				  int num = 1;
				for (int i = 1; i <= rows; i++) {
					for (int j = 1; j<=cols; j++) {
						  System.out.printf("%-3d",num++);//3 trailing space (1   2)
					}
					System.out.println();
				}
			
		} else {
			System.out.println(-2);
		}
	}
}
===================================================================================================================================
Program   		  : FOP_66
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to print tricky number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print tricky number pattern.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or  Columns  is not in a range of above constraints then, print -2.
-Otherwise to print tricky number pattern.

Sample Input1:
5 5
Sample Output1:
55555
54444
54333
54322
54321

Sample Input2:
-6 -6
Sample Output2:
-1

Sample Input3:
16 15
Sample Output3:
-2

Input4:
6 7
Output4:
7666666
7655555
7654444
7654333
7654322
7654321

Input5:
7 8
Output5:
87777777
87666666
87655555
87654444
87654333
87654322
87654321

Input6:
8 9
Output6:
988888888
987777777
987666666
987655555
987654444
987654333
987654322
987654321

Input7:
9 10
Output7:
10999999999
10988888888
10987777777
10987666666
10987655555
10987654444
10987654333
10987654322
10987654321

Input8:
11 12
Output8:
121111111111111111111111
121110101010101010101010
121110999999999
121110988888888
121110987777777
121110987666666
121110987655555
121110987654444
121110987654333
121110987654322
121110987654321
 
Input9:
5 6
Output9:
655555
654444
654333
654322
654321
 
Input10:
12 13
Ouput10:
13121212121212121212121212
13121111111111111111111111
13121110101010101010101010
13121110999999999
13121110988888888
13121110987777777
13121110987666666
13121110987655555
13121110987654444
13121110987654333
13121110987654322
13121110987654321

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 		//write the code here...
	}
} 

Solution:
=========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
			for (int i = 1; i <= rows; i++) {
					for(int j=cols;j>cols-i;j--){
						System.out.print(j);
					}
					for(int k=1;k<=cols-i;k++){
						System.out.print(rows-i+1);
					}
					System.out.println();
			}

		} else {
			System.out.println(-2);
		}
	}
}
=========================================================================================================================
Program   		  : FOP_67
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to print number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print number pattern.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or  Columns  is not in a range of above constraints then, print -2.
-Otherwise to print number pattern.

Sample Input1:
5 5
Sample Output1:
12345
23455
34555
45555
55555
 
Sample Input2:
-6 -8
Sample Output2:
-1

Sample Input3:
20 21
Sample Output3:
-2

Input4:
6 6
Output4:
123456
234566
345666
456666
566666
666666

Input5:
6 5
Output5:
12345
23455
34555
45555
55555
55555

Input6:
7 8
Output6:
12345678
23456788
34567888
45678888
56788888
67888888
78888888
 
Input7:
8 9
Output7:
123456789
234567899
345678999
456789999
567899999
678999999
789999999
899999999

Input8:
5 10
Output8:
12345678910
234567891010
3456789101010
45678910101010
567891010101010

Input9:
6 10
Output9:
12345678910
234567891010
3456789101010
45678910101010
567891010101010
6789101010101010

Input10:
7 7
Output10:
1234567
2345677
3456777
4567777
5677777
6777777
7777777

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 		//write the code here...
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
			for (int i = 1; i <= rows; i++) {
					 for(int j=i;j<=cols;j++){
						 System.out.print(j);
					 }
					 for(int k=i;k>1;k--){
						 System.out.print(cols);
					 }
					 System.out.println();
			}

		} else {
			System.out.println(-2);
		}
	}
}
=======================================================================================================================
Program   		  : FOP_68
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to print number pattern.

Input  Format  : First line contains input numbers i.e. rows and columns. 
Output Format  : Second line to print number pattern.  

Constraints:
5<=ROWS<=15
5<=COLUMNS<=15
Specification: The method numberPattern() is determined by the following rules: 
-If Rows or  Columns  is negative or zero then print -1.
-If Rows or  Columns  is not in a range of above constraints then, print -2.
-Otherwise to print number pattern.

Sample Input1:
5 5
Sample Input2:
12345
23451
34521
45321
54321

Sample Input2:
5 -5
Sample Input2:
-1

Sample Input3:
16 20
Sample Output3:
-2

Input4:
5 6
Output4:
123456
234561
345621
456321
564321

Input5:
6 7
Output5:
1234567
2345671
3456721
4567321
5674321
6754321

Input6:
7 7
Output6:
1234567
2345671
3456721
4567321
5674321
6754321
7654321

Input7:
7 8
Output7:
12345678
23456781
34567821
45678321
56784321
67854321
78654321

Input8:
8 10
Output8:
12345678910
23456789101
34567891021
45678910321
56789104321
67891054321
78910654321
89107654321

Input9:
6 10
Output9:
12345678910
23456789101
34567891021
45678910321
56789104321
67891054321

Input10:
8 8
Output10:
12345678
23456781
34567821
45678321
56784321
67854321
78654321
87654321

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		 	//write the code here..
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int rows = sc.nextInt();
		int cols = sc.nextInt();
		numberPattern(rows, cols);
	}

	public static void numberPattern(int rows, int cols) {
		if (rows <= 0 || cols <= 0) {
			System.out.println(-1);
		} else if (rows >= 5 && rows <= 15 && cols >= 5 && cols <= 15) {
			for (int i = 1; i <= rows; i++) {
					 for(int j=i;j<=cols;j++){
						 System.out.print(j);
					 }
					 for(int k=i-1;k>=1;k--){
						 System.out.print(k);
					 }
					 System.out.println();
			}

		} else {
			System.out.println(-2);
		}
	}
}
===========================================================================================
Program   		  : FOP_69
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic  to print number pattern.

Input  Format  : First line contains input numbers i.e is N. 
Output Format  : Second line to print number pattern.  

Constraints:
1<=N<=15

Specification: The method numberPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is  not in a range of above constraints then, print -2.
-Otherwise to print number pattern.
 
Sample Input1:
5
Sample Output1:
12345
21234
32123
43212
54321

Sample Input2:
-9
Sample Output2:
-1

Sample Input3:
16
Sample Output3:
-2

Input4:
9
Output4:
123456789
212345678
321234567
432123456
543212345
654321234
765432123
876543212
987654321

Input5:
6
Output5:
123456
212345
321234
432123
543212
654321

Input6:
7
Output6:
1234567
2123456
3212345
4321234
5432123
6543212
7654321

Input7:
8
Output7:
12345678
21234567
32123456
43212345
54321234
65432123
76543212
87654321

Input8:
10
Output8:
12345678910
2123456789
3212345678
4321234567
5432123456
6543212345
7654321234
8765432123
9876543212
10987654321

Input9:
-11
Output9:
-1

Input10:
13
Output10:
12345678910111213
2123456789101112
321234567891011
43212345678910
5432123456789
6543212345678
7654321234567
8765432123456
9876543212345
10987654321234
111098765432123
1211109876543212
13121110987654321

Templet:
=======
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int N = sc.nextInt();
		numberPattern(N);
		 
	}

	public static void numberPattern(int N) {
		 //write the code here...
	}
}

Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int N = sc.nextInt();
		numberPattern(N);
		 
	}

	public static void numberPattern(int N) {
		if (N <= 0) {
			System.out.print(-1);
		} else if (N >= 1 && N <=15) {
			for (int i = 1; i <= N; i++) {
				for (int j = i; j > 1; j--) {
					System.out.print(j);
				}
				for (int k = 1; k <= (N - i + 1); k++) {
					System.out.print(k);

				}
				System.out.println();
			}
		} else {
			System.out.print(-2);
		}
	}
}
==============================================================================================================
Program   		  : FOP_70
Language 		  : Java
Level    		  : Medium
Module   		  : Fundamental of Programming
Topic    		  : Control Statements 
Subtopic 		  : Loops
Problem Statement : 
For a given method write the logic to print the triangular number pattern.

Input  Format  : First line contains input numbers i.e is N. 
Output Format  : Second line to print the triangular number pattern.  

Constraints:
5<=N<=20

Specification: The method numberPattern() is determined by the following rules: 
-If N is negative or zero then print -1.
-If N is  not in a range of above constraints then, print -2.
-Otherwise print the triangular number pattern.

Sample Input1:
5
Sample Output1:
1
22
333
4444
55555

Sample Input2:
0
Sample Output2:
-1

Sample Input3:
21
Sample Output3:
-2

Input4:
7
Output4:
1
22
333
4444
55555
666666
7777777

Input5:
6
Output5:
1
22
333
4444
55555
666666

Input6:
8
Output6:
1
22
333
4444
55555
666666
7777777
88888888

Input7:
9
Output7:
1
22
333
4444
55555
666666
7777777
88888888
999999999

Input8:
10
Output8:
1
22
333
4444
55555
666666
7777777
88888888
999999999
10101010101010101010
 
Input9:
11
Output9:
1
22
333
4444
55555
666666
7777777
88888888
999999999
10101010101010101010
1111111111111111111111
 
Input10:
15
Output10:
1
22
333
4444
55555
666666
7777777
88888888
999999999
10101010101010101010
1111111111111111111111
121212121212121212121212
13131313131313131313131313
1414141414141414141414141414
151515151515151515151515151515

Templet:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int N = sc.nextInt();
		numberPattern(N);
		 
	}

	public static void numberPattern(int N) {
		 	//write the code here..
	}
}
 
Solution:
========
import java.util.Scanner;

public class Test {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int N = sc.nextInt();
		numberPattern(N);
		 
	}

	public static void numberPattern(int N) {
		if (N <= 0) {
			System.out.print(-1);
		} else if (N >= 1 && N <=20) {
			for (int i = 1; i <= N; i++) {
				 for(int j=1;j<=i;j++){
					 System.out.print(i);
				 }
				System.out.println();
			}
		} else {
			System.out.print(-2);
		}
	}
}
===============================================================================================================

 
 
 
 
 
 





