# Lazy loading
```java
// Java code to explain double check locking 
public class GFG  
{ 
  // private instance, so that it can be 
  // accessed by only by getInstance() method 
  private static GFG instance; 
  
  private GFG()  
  { 
    // private constructor 
  } 
  
  public static GFG getInstance() 
  { 
    if (instance == null)  
    { 
      //synchronized block to remove overhead 
      synchronized (GFG.class) 
      { 
        if(instance==null) 
        { 
          // if instance is null, initialize 
          instance = new GFG(); 
        } 
        
      } 
    } 
    return instance; 
  } 
} 
```
# Inner class
```java
// Java code for Bill Pugh Singleton Implementaion 
public class GFG  
{ 
  
  private GFG()  
  { 
    // private constructor 
  } 
  
  // Inner class to provide instance of class 
  private static class BillPughSingleton 
  { 
    private static final GFG INSTANCE = new GFG(); 
  } 
  
  public static GFG getInstance()  
  { 
    return BillPughSingleton.INSTANCE; 
  } 
} 
```
