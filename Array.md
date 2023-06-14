# Array
# Jagged Array :
Jagged Array is nothing but accourding to the user you can change the size of array. So for Jagged array you have to declare individual value of the internal array.
## How ro declare Jagged array:
### EX:
int arr[][]=new int[3][];   //Jagged Array declaration
		arr[0] = new int[3];        // Individual declaration of Jagged array's value
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
