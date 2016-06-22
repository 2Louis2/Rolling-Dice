# Rolling-Dice

//Die Class


public class Die {

	//public static void main(String[] args) {
		// TODO Auto-generated method stub
	
	protected final int MAX = 6;
	
	private int x = 0;
	private int faceValue;
		
	public Die()
	{
		faceValue = 1;
	}
	
	public int roll()
	{
		faceValue = (int)(Math.random() * MAX) + 1;
		return faceValue;
	}
	
	public void setFaceValue (int value)
	{
		faceValue = value;
	}

	public int getFaceValue() {
		// TODO Auto-generated method stub
		return faceValue;
	}


}

//Rolling Dice Class


public class RollingDIce {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		
		Die die1, die2;
		int sum, d1, d2;
		
		die1 = new Die();
		die2 = new Die();
		
		Die die3 = new Die ();
		
		d1 = die1.roll();
		d2 = die2.roll();
		
		System.out.println ("Die One: " + d1 + ", Die Two: " + d2);
		
		sum = die1.getFaceValue() + die2.getFaceValue();
		System.out.println ("Sum: " + sum);

	}

}
