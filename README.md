# LabTen
NMIT Lab 10 
Matthew Burton 

# 📄 Lab Ten Description
## ➡️ What is a Dynamic DataType in C#? Provide examples with your answer.
    Dynamic datatypes work much like JS datatype declaration, as JS is a dynamic language. Dynamic datatypes do not require to be initialised or given a particular datatype. 
    Dynamic datatype syntax in C#:  
                                    dynamic MyDynamicVar = 1;
                                    Console.WriteLine(MyDynamicVar.GetType()); //This would produce "System.Int32"

    This example shows how the compiler will recognise this as an int even though it has not been declared as one. 
    
## ➡️ Explain static keyword in C# and give examples of using static keyword with methods and classes.
    Static classes are sealed and therefore cannot be inherited. They cannot inherit from any class except Object. Static classes cannot contain an instance constructor. However, they can contain a static constructor.
    Class example:  static class CompanyEmployee
                    {
                        public static void DoSomething() { /*...*/ }
                        public static void DoSomethingElse() { /*...*/  }
                    }
    A static method in C# is a method that keeps only one copy of the method at the Type level, not the object level. That means, all instances of the class share the same copy of the method and its data. The last updated value of the method is shared among all objects of that Type.
    Method example: class Program  
                    {  
                        public static int myVar;  //a static field  
                        static void Main()  
                        {  
                            //Program p1 = new Program();  //a object of class  
                            myVar = 10;  
                            Console.WriteLine(myVar);  
                            Console.ReadKey();  
                        }  
                    }  