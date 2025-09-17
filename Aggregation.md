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

Object crew member is created with the Airliner, and method is there to add crew members, meaning even if we initialize the class with no crew members we can always add them from elsewhere. Allowing airliner object to have 0 crew members and still exist.