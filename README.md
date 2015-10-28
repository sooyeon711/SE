import java.io.File;
import java.io.RileReader;
import java.io.IOException;

class StuInfo{

	File stu_file = new File("C://StudentInfo//stu_Info");

	public void AddStuInfo(int id, String name, String dept, int phone){

	}
	
	public void UpdateStuInfo(int id, String name, String dept, int phone){

	}
	
	public void DeleteStuInfo(int id, String name, String dept, int phone){
	}
}

public class StudentInfo{
	public static void main(String[] args)
	{	
		FileReader info_reader = new FileReader(stu_file);
		StuInfo student = new StuInfo();
		try{
			
			char[] stu_info = new char[64];
			
			info_reader.read(stu_info);
			
		}catch(FileNotFoundException e){
			System.out.println("NOT FOUND");
		}catch(IOException e){
			System.out.println("ERROR");
		}
	}		
}	
	
	
