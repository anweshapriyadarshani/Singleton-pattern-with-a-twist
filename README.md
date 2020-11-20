# Singleton-pattern-with-a-twist
Implement the singleton pattern with a twist. First, instead of storing one instance, store two instances. And in every even call of getInstance(), return the first instance and in every odd call of getInstance(), return the second instance

class Singleton 
{ 
    private static Singleton obj; 
  
    // private constructor to force use of 
    // getInstance() to create Singleton object 
    private Singleton() {} 
  
    public static Singleton getInstance() 
    { 
        if (obj==null) 
            obj = new Singleton(); 
        return obj; 
    } 
} 
