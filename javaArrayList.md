# Java ArrayList

``
ArrayList = It is the type of , class in java
          = resizable ARRAY (special type of array)
          = inside the "java.util"  package

``
  ## methods of  ArrayList

## code :
```Java
package codingaliens.com;

import java.util.ArrayList;
import java.util.Collections;

public class ArrayListDemo {

	public static void main(String[] args) {
	    ArrayList<String> myArrayList = new ArrayList<String>();
	    myArrayList.add("coding");
	    myArrayList.add("aliens");
	     
	   //Methods of ArrayList
	    myArrayList.add("shivam");
	    myArrayList.add("shivam");
        
	    System.out.println(myArrayList.get(3));
	   
	    myArrayList.set(3,"sharma");
		   
	    System.out.println(myArrayList.contains("shivam"));
	    
	    System.out.println(myArrayList.size());
	    
	    myArrayList.remove(0);
	    //myArrayList.clear();
	    
	    //print the whole list with just name
	    System.out.println(myArrayList);
	    
	    //For each loop
	    for( String item : myArrayList)
	    	System.out.print(item+",");
	    
	    System.out.println();
	    //for,while,do-while
	    for(int i=0;i<myArrayList.size();i++)
	    	System.out.print(myArrayList.get(i)+",");
	    
	    System.out.println("\n-\---SORTING | INTEGER LIST | STRING LIST-----");
	    //INTEGER ARRAYLIST
	    ArrayList<Integer> myNumberList = new ArrayList<Integer>();
	    myNumberList.add(1);
	    myNumberList.add(10);
	    myNumberList.add(21);
	    myNumberList.add(1);
	    myNumberList.add(101);
	    myNumberList.add(91);
	    
	    //sorting number in increasing and words by alphabets
	    Collections.sort(myArrayList);
	    System.out.println(myArrayList);
	    
	    Collections.sort(myNumberList);
	    System.out.println(myNumberList);
		  
	    
	  }

}


```

## output :
````java

shivam
true
4
[aliens, shivam, sharma]
aliens,shivam,sharma,
aliens,shivam,sharma,
-----------------------SORTING | INTEGER LIST | STRING LIST-----
[aliens, sharma, shivam]
[1, 1, 10, 21, 91, 101]


````