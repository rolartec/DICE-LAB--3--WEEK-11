DICE-LAB--3--WEEK-11
====================

DICE LAB #3  WEEK #11
//  BY REINA OLARTE
//  DICE - LAB #3  -  WEEK 11


public class Dice 
{
	//  variables
	
	int COMPNumber;
	int ADDNumbers;
	int GENNumber;
	int NUMBbounces;
	int AVENumber;
	int i=1;
		public Dice(int bounces)
		{
			while(i <= bounces)
			{
				ADDNumbers += Throw();
				i++;
			}
			COMPNumber = ADDNumbers / bounces;		
		}
		public int Throw()
		{
				COMPNumber = (1	 + (int)(Math.random() * 6));
				//System.out.printf("The number that the computer generated was %d\n", computerNumber);
				return COMPNumber;
		}
		public int Throw(int bounces)
		{

			NUMBbounces = bounces;
			
			while(i <= bounces)
			{
				GENNumber = (1+(int)(Math.random() *6));
				
				System.out.printf("The generated number is: %d\n", GENNumber);
				
				ADDNumbers += GENNumber;
				
				System.out.printf("The Sum of the Number: %d\n\n", ADDNumbers);
				
				i++;
			}
			COMPNumber = ADDNumbers / NUMBbounces;
			
			return COMPNumber;
		}
		public int Value()
		{
			return COMPNumber;
		}
}
