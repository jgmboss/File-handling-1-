import java.io.FileReader;
import java.io.IOException;
import java.io.BufferedReader;
public class filereading
{
     public static void main (String[] args) throws IOException{
        FileReader fReader = new FileReader("U:\\Computer Science\\Filehanding\\1)a.txt");
        BufferedReader bReader = new BufferedReader(fReader);
        
        String text = bReader.readLine();
        
        do{ 
            System.out.println(text);
        } while ((text = bReader.readLine()) != null);
        
        bReader.close();
}
}
