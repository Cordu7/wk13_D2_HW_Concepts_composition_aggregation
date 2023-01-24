# Polymorphism & Composition Homework - Quiz

# Polymorphism

1. What does the ___word___ 'polymorphism' mean?

It means more than one form

2. What does it mean when we apply polymorphism to OO design? Give a simple Java example.

It means that an object has more than one type. that means it can be grouped by these different types. E.g an Object can be put in an array with its class or its superclass if it has a superclass.

public abstract class ReadingMaterial{

  private String name;

  public(String name){
    this.name = name;
  }
}


public class Book extends ReadingMaterial{
  public Book(Sting name){
    super(name);
  }
}

Alternatively an object can be polimorphic because it instantiates an interface which means it is an object of that interface type. An interface is promising a behaviour which is instantiated by the object's class.

3. What can we use to implement polymorphism in Java?

superclasses/classes
classes/interfaces

4. How many 'forms' can an object take when using polymorphism?

as many as it has different types if it consists of 5 interfaces and one superclass then that would make 7 (it also has the form of it's own class)

5. Give an example of when you could use polymorphism.

When I want to instantiate interfaces in a class
when a class inherits something from a superclass.



# Composition and Aggregation

6. What do we mean by 'composition' in reference to object-oriented programming?

Composition means that an object is composed of different parts which importantly are constitutive of the object. This means the parts cannot exist outwith of the objects scope.

7. When would you use composition? Provide a simple example in Java.

Composition is used when an object contains of different types. The cover cannot exist without the book.


public class Cover{

  private String title;
  private String author;

  public Cover(Sting title, String author){
    this.title =  title;
    this.author = author;
  }


}

public abstract class ReadingMaterial{

  private Cover cover
  private String name;

  public(Cover cover, String name){
    this.cover = cover;
    this.name = name;

  }
}



8. Give a difference between composition and aggregation?

Both have are a 'has a' relationship, but composition is a stronger relation than aggregation.

aggregation is a relationship where the two types which hold the relationship can exist independently even it the relationship is broken.

Composition is a relation where one type will cease to exist if the other type does not exist any more.

9. What is/are the advantage(s) of using composition/aggregation?

with composition:
-an object becomes polymorphic.

with aggregation:

10. When using composition, when an object is destroyed, what happens to all the objects it is composed of?

they are also destroyed.

11. When using aggregation, when an object is destroyed, what happens to all the objects it is composed of?

They continue to exist independently as they are not dependent on each other.
