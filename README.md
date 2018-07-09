# CareerDevsInterviewQuestions

Start time:
End Time:

Hi Everyone,

Here are your interview questions. There are four sections:

Algorithms,
Object Oriented Programming
Design Patterns
.Net (skip if not applicable to your learning track)
Java (skip if not applicable to your learning track)

Please set aside two hours to complete this exercise.  Please set a timer and note your start time and your end time.  This isn’t a race, but it will help you as well as careerdevs to determine how long it takes for you to complete this assignment. 
By mastering the underlying concepts AS WELL AS the answers to the following interview, you will be more than prepared to crush your job interview.

Please mark all difficult questions with a “D!”.  This will help us know what we need to focus more on in the future.  Thanks and congrats on Killing your upcoming software developer job interview!

Talk soon,

Arnell

Algorithms:

1. What is Big O notation?  Be descriptive (4 or more sentences).  What are its various permutations?
Your answer:
> Big-O notation is a way of expressing a function's space and time consumption.  How does a function’s performance scale as the input size grows to infinity?  To meaningfully compare algorithmic performance, we compare the asymptotic behavior of algorithms.  Big-O usually describes the upper bound on the growth rate of the function.

2. What are Divide and Conquer algorithms? Describe how they work. Can you give any common examples of the types of problems where this approach might be used?
Your Answer:
> A divide and conquer algorithm is a recursion algorithm.  
They work by defining a function or calculating a number by repeating the application of an algorithm, until it is simple enough to be solved directly. 
The solutions to the sub-problems are then combined to give a solution to the original problem.  For example, 

3. What is a Hash Table, and what is the average case and worst case time for each of its operations? How can we use this structure to find all anagrams in a dictionary?
Your Answer: 
>A hash table is an array data structure that can map keys to values.
The key is hashed and the resulting value is used as the index at which to store the value within the array.
Note that it is best to use prime numbers for the array size because it helps to avoid collisions.
The average cost for each lookup is independent of the number of elements stored in the table because it calculates the index instead of searching for the value.
Therefore, the average and worst case for space is O(n).  Average search, insert and delete is O(1), and O(n) for worst case search, insert and delete.
Since the hash algorithm would produce the same result for anagram words, like stressed == desserts, hashing words would result in the same index, so an anagram is found.

4. Why would you use a Binary Search for a linked lists?
Your Answer:
> You would use a Binary Search for a linked lists if it is a sorted linked list, otherwise what would be point applying a Divide and Conquer Algorithm to an unsorted list?  Because linked list is dynamic and not contiguous, finding the middle element is difficult.  You could use a Skip List Algorithm, which would reduce the time complexity from O(n) to O(sqroot(n)).  A Skip List Algorithm allows you to speed ahead to  a section of the linked list where the node you’re searching for is likely to be.

5. Given a large string of characters, what is the most efficient way to identify the first unique character in the string?
Your Answer:
> When you scan the string and construct a count array, also store the index of the first time a character is encountered.  
Then you can scan the count array to find the first non-repeating character.

6. What is a logarithm?  Be descriptive (4 or more sentences).
Your Answer:
> A logarithm is the inverse of the exponential function.  
Specifically, the logarithm returns the value of the exponent required to raise the use to a specified value.  
For example, log2 64 = 6 because 2**6 = 64 (that’s 2 exponent 6) or more generally, loga b = c means a**c = b

7. Explain O(log N)? Be descriptive (4 or more sentences).
Your Answer:
> O(log n) means the algorithm’s running time is dependent on the logarithm of the input size.  
Logarithms in computer science is usually in base 2 unless specified otherwise, so log2 n means what exponent does 2 need to be raised to to equal n?

8. How does algorithmic mastery make one a better computer scientist and software engineer?  Be descriptive (4 or more sentences).
> Algorithms are the building blocks of computer programs.  
They are the road map to solving a problem.  
One of the most important aspects of an algorithm is how fast it is, as represented by its runtime relative to the size of the input.
 
9. What is the relationship between Dijkstra's algorithm and graph data structures.
Your Answer:
> Dijkstra's algorithm is for finding the shortest paths between nodes in a graph, which may represent, for example, road networks.
This youtube video explains it well.  https://www.youtube.com/watch?v=bum_19loj9A&list=PLBZBJbE_rGRV8D7XZ08LK6z-4zPoWzu5H


10. Read some of the following.  What did you find interesting?
http://delivery.acm.org/10.1145/1290000/1283927/a1972-dijkstra.pdf?ip=68.0.213.32&id=1283927&acc=OPEN&key=4D4702B0C3E38B35%2E4D4702B0C3E38B35%2E4D4702B0C3E38B35%2E6D218144511F3437&__acm__=1530763760_2fe16c6dd019b5fc00fe92f4fc664579
Your answer:
> An error occurred while processing your request.
Reference #50.cd58db17.1531096753.1db6f6cb  
The link does not work

11. Watch some of the following. 
Who was the person speaking at the start of the video?  Elaborate.
Your answer:
> Eric Schmidt vp of the general Systems Group of Sun Microsystems introduced Dr. Edsger W. Dijkstra - Reasoning about programs
The general structure of correctness and separation of concerns between total correctness and partial correctness and termination.
Total correctness means the program will produce the right result.
Partial correctness will produce the right result if its execution terminates.
To explain, he presented the general pattern that will prove things about the repetitive construct do B until the negation of the post condition P.

What did you find interesting about the lecture?
https://www.youtube.com/watch?v=GX3URhx6i2E
Your answer:


12. List two resources for learning about/exploring algorithms (url) ?
> A. https://brilliant.org/courses/computer-science-algorithms/  
B. https://www.geeksforgeeks.org/fundamentals-of-algorithms/

13. List a url to an algorithm repository along with a snippet of code. 
>A (url1).https://github.com/TheAlgorithms/Java/blob/master/Misc/PalindromicPrime.java

B. Code snippet:
>   public static boolean prime(int num) { // checking if number is prime or not
        for (int divisor = 2; divisor <= num / 2; divisor++) { 
            if (num % divisor == 0) { 
                return false; // false if not prime
            } 
        } 
        return true; // True if prime
    } 

C. Describe the algorithmic context of the code snippet pasted above
> This algorithm checks if the argument is a prime number
The for loop counts from 2 (1 would make no sense) to one half of the number passed in (because you only have to go half way then you wrap around)
If the argument modulo the counter is not equal zero, then it is a prime number, otherwise the for loop would exit prematurely and so the argument is not a prime number.

14. List a second url to an algorithm repository along with a snippet of code.  
A (url1). 
> https://www.geeksforgeeks.org/biginteger-class-in-java/

B. Code snippet:

    // Returns Factorial of N
        static BigInteger factorial(int N){
        // Initialize result
        BigInteger f = new BigInteger("1"); // Or BigInteger.ONE
  
        // Multiply f with 2, 3, ...N
        for (int i = 2; i <= N; i++)
             f = f.multiply(BigInteger.valueOf(i));
      
            return f;
        }

C. Describe the algorithmic context of the code snippet pasted above    
> This algorithm is used for mathematical operation which involves very big integer calculations that are outside the limit of all available primitive data types.
    The for loop multiplies the argument iteratively from 2 to N then returns the factorial of that big Integer


# Design Patterns

1. What is a design pattern? Be descriptive (6 [six] or more sentences).
Your answer:
> In software engineering, a design pattern is a general, reusable solution to a commonly occurring problem in software design.  
It is a description or a template for how to solve a problem that can be used in many different situations.
Object-oriented design patterns typically show relationships and interactions between classes or objects, without specifying the final application classes or objects that are involved.
Design patterns may be viewed as a structured approach to computer programming.
They are somewhere between a programming paradigm and an algorithm.

2. What is the purpose of  design pattern? Be descriptive (4 or more sentences).
Your answer:    
> Design patterns can speed up the development process by providing tested, proven development paradigms.  
Freshly written code can have hidden subtle issues that take time to be detected.
Reusing design patterns can help to prevent such subtle issues.
It also improves code readability for coders and architects who are familiar with the patterns.


3. How does design pattern mastery make one a better computer scientist and software engineer?  Be descriptive (4 or more sentences).
Your answer:  
> Design patterns make it easier to reuse successful designs and architectures.  
Expressing proven techniques as design patterns makes them more accessible to developers of new systems.  
Design patterns help you choose design alternatives that make a system reusable and avoid alternatives that compromise reusability.


4. How do design patterns relate to OOP?
Your answer:  
> Design patterns help you identify less-obvious abstractions and the objects that can capture them.  
Objects that represent a process or algorithm don't occur in nature, yet they are a crucial part of flexible design.
The Strategy pattern describes how to implement interchangable families of algorithms.  
The State pattern represents each state of an entitiy as an object.  
These objects are seldom found during analysis or even in the early stages of design; they are discovered later in the course of making a design more flexible and reusable.

5. Describe the MVC design pattern and include a use case.  Be descriptive (4 or more sentences).
Your answer:  
> MVC is a triad of three kinds of  objects:  
Model is the application object.  
View is the screen presentation.  
Controller defines the way the user interface reacts to user input.


6. Name and describe another design pattern and include a use case.  Be descriptive (4 or more sentences).
Your answer:
> Factory Method pattern defines an interface for creating an object, but lets the subclasses decide which class to instantiate.

7. Name and describe another design pattern and include a use case.  Be descriptive (4 or more sentences).
Your answer:  
> Observer pattern defins a one-to-many dependency between objects so that when one object changes state, all its dependents are notified and updated automatically.  
Think ajax in JavaScript.

Object Oriented Programming

1. What is a Object Oriented Programming? Be descriptive (6 [six] or more sentences).
Your answer:

2. What are the goals of OOP?
3. Define Encapsulation
Your answer:

Paste a commented code snippet example below: 

4. Define Abstraction 
Your answer:

Paste a commented code snippet example below: 

5. Define Inheritance
Your answer:
Paste a commented code snippet example below: 
6. Define Polymorphism
Your answer:

Paste a commented code snippet example below: 

7. Give a code example of an Object being declared, then instantiated and then initialized.

8. What is the Diamond Problem as it relates to:
A. C#
B. Java
> A class cannot inherit from two parents because if there was a method with the same name, the compiler would not know which one to use.

9. What is the difference between polymorphism and inheritance?
Your answer:
10. What is Association?
Your answer:
11. What is Aggregation?
Your answer:
12. What is Composition?
Your answer:
13. What are constructors and what are destructors?
Your answer:

14. What are constructors and what are destructors?
Your answer:
15. What are access modifiers?
 

.Net Questions

1. What are the different types of classes in C#?
2. Explain Code compilation in C#
3. What are the differences between a Class and a Struct?
4. What is the difference between Virtual method and Abstract method?
5. How is Exception Handling implemented in C#?
6. What are C# I/O Classes? What are the commonly used I/O Classes?
7. What are Boxing and Unboxing?
8. What is a String? What are the properties of a String Class?
9. Give an example of using a sealed class in C#?
10. What is the difference between “finalize” and “finally” methods in C#?
11. Why and when should you use each of them?
12. Describe compilation in C#?
13. What is the difference between an abstract class and an interface?

14. What is a delegate in .NET?
 

# Java Questions

1. Explain public static void main(String args[]).
> public is an access specifier
static is access modifier
void is return type that does not return any value
main is the method name

2. Explain public static void main(String args[]).
3. Why java is not 100% Object-oriented?
4. What are wrapper classes?
5. What is singleton class and how can we make a class singleton?
6. What is the difference between equals() and == ?
7. What are the differences between Heap and Stack Memory?
8. What is runtime polymorphism or dynamic method dispatch?  Create an example with comments. 
9. What is method overloading and method overriding?
10. What is multiple inheritance? Is it supported by Java? (dejavu?)
11. What is a servlet?
12. List five features of Java?
13. List some Java keywords(unlike C,C#, C++ keywords)?
14. When would you use the parseInt() method ?
15. Which package is used for pattern matching with regular expressions?
16. Describe the super keyword?
17. Does Java support multiple inheritance. Why or Why not?
> No, Java does not support multiple inheritance because if a class had two parents and each had a method with the same name, the compiler would not know which one to use.

18. Name AND DEFINE each of the methods of Object Class