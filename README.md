import java.io.File;
import java.io.FileWriter;
import java.io.IOException;

public class Jala {
	public static void main(String[] args) throws IOException 
  {
		File file = new File("myfile.txt");
		FileWriter fr = new FileWriter(file);
        try
        {
          fr.write("Hi Im sai!!!");
        } catch (IOException e) {
            System.out.println("Sorry!!! can't read the file");;
        }
        fr.close();
   }
}
