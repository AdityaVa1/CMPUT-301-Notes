Takes repeated/common/shared characteristics between two or more classes and factors them out into another class.

![[UML_Generalization.png]]

The solid line shows inheritance, the arrow points to the superclass.

```javaScript
public abstract class Animal {
	protected Int numberOfLegs;
	protected Int numberOfTails;
	protected String name;
	
	public Animal (String petName, int legs, int tails) {
		this.name = petName;
		this.numberOfLegs = numberOfLegs;
		this.numberOfTails = numberOfTails;
	}
	
	public void walk() {..}
	public void run() {..}
	public void eat() {..}
}
```

Since the Animal class is a generalization it should never be created as an object on its own, hence we use abstract.