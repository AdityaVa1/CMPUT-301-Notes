Indicates a strong "has-a" relationship between two [[UML Diagrams]]. Meaning the whole cannot exist without its parts, and vice versa. In this you can typically access the parts through the whole.

![[UML_Decomposition_Composition.png]]

```javascript
public class House {
	private Room room;
	
	public House() {
		room = new Room();
	}
}
```