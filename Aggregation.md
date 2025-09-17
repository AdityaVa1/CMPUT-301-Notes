Indicates a weak "has-a" relationship between two [[UML Diagrams]]. A whole has parts from another object that belong to it. However, this is a weak relationship, meaning that if one is deleted the other can still exist without it.

![[UML_Decomposition_Aggregation.png]]

```javascript
public class Airliner {
	private ArrayList<CrewMember> crew;
	
	public Airliner() {
		crew = new ArrayList<CrewMember>();
	}
	
	public void add (CrewMember crewMember) {
		...
	}
}
```
