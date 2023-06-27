# Array
# Jagged Array :
Jagged Array is nothing but accourding to the user you can change the size of array. So for Jagged array you have to declare individual value of the internal array.
## How ro declare Jagged array:
### EX:
		int arr[][]=new int[3][];   //Jagged Array declaration
		arr[0] = new int[3];        // Individual declaration of Jagged array's value.
		arr[1] = new int[2];
		arr[2] = new int[5];

		//take arandom input for Jagged array
		for(int i =0; i<arr.length;i++){
		  for(int j=0; j<arr[i].length;j++){
		    arr[i][j] = (int)(Math.random()*10);
		    System.out.print(arr[i][j]+ " ");
		    }
		 System.out.println();
		   }


# Array of Objects :
Create an object of a class and then assign those objects to an Array
### Ex:
	class Student{
	int rollNo;
	String name;
	float marks;
	}

	public class ArrayOfObjects {

	public static void main(String[] args) {
		//Create a student object and then assign those objects to an Array
		
		//Create an object of student class
		Student s1 = new Student();
		//declare values to the object
		s1.rollNo = 001;
		s1.name = "Gudul";
		s1.marks = 80;
		
		Student s2 = new Student();
		s2.rollNo = 002;
		s2.name = "Fudul";
		s2.marks = 85;
		
		Student s3 = new Student();
		s3.rollNo = 003;
		s3.name = "Dudul";
		s3.marks = 95;
		
		//Here we are not creating an object
		//here we are creating an array which is holding the reference of an object
		Student Students[] = new Student[3];
		Students[0] = s1;
		Students[1] = s2;
		Students[2] = s3;
		
		//Print the values of the Student
		for(int i =0;i<Students.length;i++) {
			System.out.println(Students[i].name + " " +Students[i].rollNo + " " + Students[i].marks);
		}
	}

}
