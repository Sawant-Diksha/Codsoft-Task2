# Codsoft-Task2

import java.util.*;
class StudentGradeCalci 
{
	public static void main(String[] args) 
	{
		Scanner sc=new Scanner(System.in);
		System.out.println("HOW MANY SUBJECTS DO YOU HAVE??....");
		int no_of_subjects=sc.nextInt();
		String subject[]=new String[no_of_subjects];
		
		int Total=0;
		double percentage=0.0;
		for (int i=0;i<no_of_subjects ;i++)
		{
			
			System.out.println("ENTER THE SUBJECT NAME "+(i+1)+":");
			 subject[i]=sc.next();
			System.out.println("ENTER THE MARKS OF "+subject[i]);
			 int marks=sc.nextInt();
			 Total=Total+marks;
			 percentage=((double)Total/(no_of_subjects*100))*100;
			 
		}
	
		char grade;
		
		if (percentage>=90 && percentage<=100)
		{
			grade='A';
			System.out.println("***********....RESULT....***********");
			System.out.println("===================================");
			System.out.println("\n\t1.TOTAL MARKS ::"+Total+"\n\t2.PERCENTAGE  ::"+percentage+"%\n\t3.GRADE       ::"+grade);
			System.out.println("===================================");
			
		}
		else if (percentage>=70 && percentage<=90)
		{
			grade='B';
			System.out.println("***********....RESULT....**********");
			System.out.println("===================================");
			System.out.println("\n\t1.TOTAL MARKS ::"+Total+"\n\t2.PERCENTAGE  ::"+percentage+"%\n\t3.GRADE	      ::"+grade);
			System.out.println("===================================");
				
		}
		else if (percentage>=50 && percentage<=70)
		{
			grade='C';
			System.out.println("***********....RESULT....**********");
			System.out.println("===================================");
			System.out.println("\n\t1.TOTAL MARKS ::"+Total+"\n\t2.PERCENTAGE  ::"+percentage+"%\n\t3.GRADE	      ::"+grade);
			System.out.println("===================================");
		}
		else if (percentage>=35 && percentage<=50)
		{
			grade='D';
			System.out.println("***********....RESULT....**********");
			System.out.println("===================================");
			System.out.println("\n\t1.TOTAL MARKS ::"+Total+"\n\t2.PERCENTAGE  ::"+percentage+"%\n\t3.GRADE	     ::"+grade);
			System.out.println("===================================");
		}
		else 
		{
			grade='F';
			System.out.println("***********....RESULT....**********");
			System.out.println("===================================");
			System.out.println("\n\t1.TOTAL MARKS ::"+Total+"\n\t2.PERCENTAGE  ::"+percentage+"%\n\t3.GRADE	      ::"+grade);
			System.out.println("===================================");
		
		}
		
	}
}
