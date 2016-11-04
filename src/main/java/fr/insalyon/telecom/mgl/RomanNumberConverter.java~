public class RomanNumberConverter {

	static private int convertOne(char rNumber){
		switch(rNumber){
			case 'I' : return 1; 
			case 'V' : return 5;
			case 'X' : return 10;
			case 'L' : return 50;
			case 'C' : return 100;
			case 'D' : return 500;
			case 'M' : return 1000;
			default : return 0;
		}	
	}

	static int convert(String romanNumber){
		int n=romanNumber.length();
		int converti=0;
		for(int i=0; i<n-1;i++){
			int a=convertOne(romanNumber.charAt(i));
			int b=convertOne(romanNumber.charAt(i+1));
			if(a<b){
				converti=converti-a;
			}
			else{
				converti=converti+a;
			}
		}
    converti=converti+convertOne(romanNumber.charAt(n-1));
		return converti;

	}


	String convert(int number){
		return null;
	}

	public static void main (String[] args){
		if (args[0]!=null){		
			int i=0;
			i = convert(args[0]);
		  System.out.println(args[0]+" = "+i);
		}
		else{
			System.out.println("pas d'argument");
		}
	}	
}
