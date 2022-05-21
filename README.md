# Midterm-Project_UML-Class-Diagram
 
Magandang araw sa po sa lahat. Ngayon ay aming ipiprisinta ang aming nagawang java project about Unified Modeling Language.

package umlClassDiagram;//Gumawa kami ng package-info.java sa source file na
Project/src import java.io.;//import java.io. statement tells the compiler where to look for the external classes you use in your code. It needs to find them to check that you are using them correctly, calling methods that exist, passing the right arguments to them, etc.

//If you import java.io.* the compiler will look at all classes in      
  the java.io package when it needs to find a class you are using.  
  It will actually look for the .class files in the java\io    
  directory (and in this directory path inside any jar files) on the 
  classpath.
               This particular import happens to be the Java Input/Output package 
               containing the .class files for reading and writing data.
            If you used one of the classes in this package without the import    
               statement (and without explicitly specifying its package when you 
               used it), the compiler would be unable to find it and would output 
               an error message 'Cannot resolve symbol, class Xxxxx'. This also 
               happens if the .class files you try to import are not actually 
               present in the package directory or in a jar file on the 
               classpath.

             //Upon reading the Java development guide about Creating first Java 
               Project in the help section we were prompted to download 
               (JUnit3.8.1src)at inimport namin dito 
               sa project. JUnit is an open source unit testing framework for 
               Java. Hindi namin mapa-run itong program bago namin malaman sa  
               help section ng eclipse na kailangan pala idownload at iimport ito      
               sa ginawang project 
public class Menu {//Gumawa kami ng class Menu na naka-public modifier //Pumunta naman po tayo sa mga methods na ginamit namin. Una ay ang public
static void main String args na may throws Exception. public static void main(String []args)throws Exception {//public : it is a access specifier that means it can be accessed by any other class in the program. static : it is access modifier that means when the java program is
load then it will create the space in memory automatically. void(return type) : it does not return any value. main() : it is a method or a function name.(First method to execute by JVM)- Java Virtual Machine is a virtual machine that enables a computer to run Java programs as well as programs written in other languages that are also compiled to Java bytecode. string args[] : its a command line argument it is a collection of
variables in the string format. throws Exception : Use exceptions to notify about things that should not be ignored. Exceptions are more than control flow mechanisms.
They give to the (method) client useful information about exceptional outcomes that they must be aware of and handled. Gumamit kami ng throws Exception para magbigay ng warning message
kapag ang hinihinging impormasyon na dapat iinput ay wala sa mga
mapagpipilian during run time. String order, again;//declaring variables "order" and "again" na naka string na data types

  //Calling method BufferedReader for object “br”. 
 BufferedReader class of the java.io package can be used with other readers to   
    read data (in characters) more efficiently
 BufferedReader input = new BufferedReader (new InputStreamReader   
   (System.in)); Once we have created a BufferedReader we can use its method  
   readLine() to read one line of characters at a time from the keyboard and 
   store it as a String object    
   BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
			int price1=0, loop1=0, quantity1;
			int total = 0, payment = 0, ans = 0;
//We used primitive data type “int” to declare 
   Variables price1m, loop1, quantity1, totat, payment and     
   ans. It can also be used with methods to return integer   
   type values
	        
	        System.out.println(">>");
	        System.out.println("WELCOME SA AMO KARENDERYA");
	        System.out.println(">>");
	        System.out.println("                           MENU ");
		    System.out.println(" ______________________________________________________"); 
			System.out.println("| Code        | Meal                       | Price     |");
			System.out.println("*******************************************************");
			System.out.println("| (A1)        | Mediterranean pork chops   | P30.00    |");
			System.out.println("| (A2)        | Lemon herb orzo            | P139.00   |");
			System.out.println("| (B1)        | Greek chicken meatballs    | P35.00    |");
			System.out.println("| (B2)        | Bacon-wrapped asparagus    | P50.00    |");
			System.out.println("| (C1)        | Oven roasted tomatoes      | P65.00    |");
			System.out.println("| (C2         | Mashed potato puffs        | P79.00    |");
			System.out.println("| (D1)        | Chicken lyonaise           | P60.00    |");
	    	System.out.println("| (D2)        | Creamy barley soup w/ dill | P40.00    |");
			System.out.println("| (E1)        | Baklava                    | P10.00    |");
			System.out.println("| (E2)        | Beef tenderloin            | P50.00    |");
			System.out.println("| (E3)        | Sourdough                  | P70.00    |");
			System.out.println("| (F1)        | Faux gras                  | P50.00    |");
			System.out.println("| (F2)        | Red mullet                 | P10.00    |");
			System.out.println("*******************************************************");
//Yung mga lines of codes containing method System.out.println ay ang aming presentasyon para ipakita yung mga Food Menu each with its Code, Price, and name of Meal System. out. println is a Java statement that prints the argument passed, into the System. Out. This method displays the result on the screen based on the parameter passed to it do {

				System.out.println("");
				System.out.print("Enter code order:");
				order = br.readLine();
				//”br” object which assigned to BufferedReader is being called to method .readLine to passed it in object “order”. The readLine(String fmt, Object args) method is a static method of Java Console class. It is used to provide a formatted prompt, then reads a single line of text from the console.
//Now its time to select your order sir! By using object “order” for Menu selection we can find your order in the list thanks to if else conditional statement and
Java String equalsIgnoreCase() method. The method equalIgnoreCase() compares two strings, ignoring case differences. If the strings are equal, equalsIgnoreCase() returns true. If not, it returns false. if(order.equalsIgnoreCase("A1")) { price1 = 30; System.out.println("Order Description: Mediterranean pork chops "); } else if(order.equalsIgnoreCase("A2")) { price1 = 139; System.out.println("Order Description: Lemon herb orzo"); } if(order.equalsIgnoreCase("B1")) { price1 = 35; System.out.println("Order Description: Greek chicken meatballs"); } else if (order.equalsIgnoreCase("B2")) { price1 = 50; System.out.println("Order Description: Bacon-wrapped asparagus"); } else if (order.equalsIgnoreCase("C1")) { price1 = 65; System.out.println("Order Description: Oven roasted tomatoes"); } if (order.equalsIgnoreCase("C2")) { price1 = 79; System.out.println("Order Description: Mashed potato puffs"); } else if(order.equalsIgnoreCase("D1")) { price1 = 60; System.out.println("Order Description: Chicken lyonaise"); } if(order.equalsIgnoreCase("D2")) { price1 = 40; System.out.println("Order Description: Creamy barley soup w/ dill"); } else if (order.equalsIgnoreCase("E1")) { price1 = 10; System.out.println("Order Description: Baklava"); }

				if(order.equalsIgnoreCase("E2")) {
							         price1 = 50;
							         System.out.println("Order Description:  Beef tenderloin");
				}			       
			    else if(order.equalsIgnoreCase("E3")) {
							        	 price1 = 70;
	                                   System.out.println("Order Description:  Sourdough");
			    }
				if(order.equalsIgnoreCase("F1")) {
							 price1 = 50;
							System.out.println("Order Description:  Faux gras");
				}
				else if(order.equalsIgnoreCase("F2")) {
							  price1 = 10;
							  System.out.println("Order Description:  Red mullet");
				
				}
							  
				System.out.println("Enter Quantity:");
				quantity1 = Integer.parseInt(br.readLine());
				     total += price1*quantity1;
				System.out.print("another order?(Y/N): ");
				again = br.readLine();
				
				if (again.equalsIgnoreCase("y"))
					loop1 = loop1+1;
				else loop1 = loop1- 100;
				
			
		}
//Why there is do-while loop in our program? Simply because we want you sir to order food as many as you can afford and share it with us. If you select Y stands for yes! meaning the condition becomes true then loop does its work for you to add another order. It only stops when stomach is full. No I mean if you type or inputed N which stands for NO in this case loop becomes false and loop stops. The Java do-while loop is used to iterate a part of the program repeatedly, until the specified condition is true. If the number of iteration is not fixed and you must have to execute the loop at least once, it is recommended to use a do-while loop. Java do-while loop is called an exit control loop. //Inside do-while loop we also added how to compute the total price for multiple orders. In this case we use the equation total += price*quantity and calling method Integer.parseInt(br.readLine()) and assign to quantity1 variable.

			while(loop1==1) ;
			
			
			System.out.println("SERVICE CREW COUNTER");
			System.out.println("Total Price:"+total);
			
			
			System.out.print("Enter Payment:");
			payment = Integer.parseInt(br.readLine());
			ans = payment - total;
			if(total<payment) {
				System.out.println("Your change is:"+ans);
				System.out.println("Thank you for your order!");
			}
			else if (payment<total) {
				System.out.println("Luhh kulang...!Luhh");
//Multiple lines of codes after do-while loop is about Payment. Gumamit din kami dito ng conditional statement para ipakita and output kung kulang or subra ang naibayad. Kung sobra then yung output is yung sukli at kung kulang mayroon cute na mensahing lalabas.

//At dito po nagtatapos ang aming presentasyon sa aming proyekto sa programming. Maraming thank you! At muli, magandang araw sa lahat. }

			}
	}    
