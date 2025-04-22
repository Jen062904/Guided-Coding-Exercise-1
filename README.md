# Guided-Coding-Exercise-1
Objective:
Define and differentiate compile-time polymorphism.
Implement method overloading in Java.

File Naming Convention:
MethodOverloadingDemo.java

Step 1: Create a Java File
Create a new Java file named MethodOverloadingDemo.java.
This file will contain your Java code for this exercise.

Step 2: Define the main Method
Inside the file, create the main method. This is the entry point of your Java program.

Snippets
public class MethodOverloadingDemo {
    public static void main(String[] args) {
        // Code will go here
    }
}


Step 3: Create the Calculator Class
Create a new class named Calculator in the same file (or in a separate file named Calculator.java).

Snippets
class Calculator {
    // Methods will go here
}


Step 4: Implement Overloaded add() Methods
Inside the Calculator class, create three overloaded add() methods:
add(int a, int b): Takes two integers as arguments and returns their sum.
add(int a, int b, int c): Takes three integers as arguments and returns their sum.
add(double a, double b): Takes two double values as arguments and returns their sum.

Snippets
// Overloaded method #1: Adds two integers.
public int add(int a, int b) {
    return a + b;
}

// Overloaded method #2: Adds three integers.
public int add(int a, int b, int c) {
    return a + b + c;
}

// Overloaded method #3: Adds two double values.
public double add(double a, double b) {
    return a + b;
}



Step 5: Call Overloaded Methods in main()
Inside the main() method of the MethodOverloadingDemo class, create an instance of the Calculator class.

Snippets
Calculator calc = new Calculator();


Call the overloaded add() methods with different arguments to demonstrate method overloading:
Call calc.add(10, 20) and display the result.
Call calc.add(10, 20, 30) and display the result.
Call calc.add(10.5, 20.5) and display the result.

Snippets
System.out.println("Sum of two ints: " + calc.add(10, 20));
System.out.println("Sum of three ints: " + calc.add(10, 20, 30));
System.out.println("Sum of two doubles: " + calc.add(10.5, 20.5));


Step 6: Compile and Run
Save the file(s) as MethodOverloadingDemo.java (and Calculator.java if you created it separately).
Compile the code:

Windows Terminal
javac MethodOverloadingDemo.java


Run the compiled code:

Windows Terminal
java MethodOverloadingDemo


Notable Observations:
Method overloading allows you to define multiple methods with the same name but different parameter lists within the same class.
The Java compiler determines which overloaded method to call based on the arguments passed at compile time. This is known as compile-time polymorphism or static polymorphism.
Method overloading improves code readability and reusability by providing a consistent interface for similar operations on different data types or numbers of arguments.

Java Programming Best Practices:
Use method overloading when you have similar operations that need to be performed on different data types or with different numbers of parameters.
Choose meaningful method names that clearly indicate the purpose of the operation.
Ensure that the parameter lists of overloaded methods are distinct enough to avoid ambiguity during compilation.

Conclusion:
This exercise demonstrated method overloading in Java, a key feature that enables compile-time polymorphism. You learned how to create overloaded methods with different parameter lists and how the compiler resolves method calls based on the provided arguments. Method overloading promotes code organization and flexibility by allowing you to define a single method name for related operations on different data types or numbers of parameters.
