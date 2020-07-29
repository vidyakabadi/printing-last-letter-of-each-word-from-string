# printing-last-letter-of-each-word-from-string
Create a class Solution which contains main method. -> Read a String with spaces between them (String) -> Print last character of each word without changing the case of the character -> Print all the characters in a single line  Input Hello World! This is my TCS Program Output o!ssySm


import java.util.Scanner;
public class Main
{
	public static void main(String[] args) {
	    Scanner sc=new Scanner(System.in);
	    String s=sc.nextLine();
	    String res="";
	    for(int i=0;i<s.length();i++)
	    {
	        if(s.charAt(i)==' ')
	        {
	            res=res+s.charAt(i-1);
	        }
	    }
	    res=res+s.charAt(s.length()-1);
		System.out.println(res);
	}
}
