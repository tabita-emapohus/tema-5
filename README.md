import java.io.BufferedReader;
import java.io.FileReader;
import java.io.FileWriter;
import java.io.IOException;

public class Intervale {
	private double inc;
	private double sfr;
	private int totalnum;
	private int numintr;
	
	public Intervale(double inc, double sfr) {
		this.inc = inc;
		this.sfr = sfr;
		this.totalnum = 0;
		this.numintr = 0;
	}
	public void testNum (Double num) {
		totalnum++;
		if(num >= inc && num <= sfr) {
			numintr++;
		}
	}
	public double calcProcent() {
		if(totalnum == 0) {
			return 0;
		}
		else 
		{
			return numintr/totalnum*100;
		}
	}
	public static void main(String[] args) {
	try {
		BufferedReader reader = new BufferedReader (new FileReader("numere.dat.txt"));
	    FileWriter writer = new FileWriter("statistica.dat");
	    
	}
     catch (IOException e) {
    	 
     }
	

	}

}
