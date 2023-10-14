---
description: An Object is simply any object within a level.
---

# Object

## Definition

Objects can be stored singularly using the Object variable type. Objects have properties which can be accessed by specialized nodes.

## Related Nodes (Methods)

Below are the Nodes that accept an Object parameter.

### Data Nodes

Retrieves data about a given Object.

* Convenience
  * Get Object Position \[Vector3]
  * Get Object Rotation \[Vector3]
  * Is Valid Object \[Boolean]
* Stored Variables
  * Get \[Type] Variable

{% hint style="info" %}
Objects can store variables with a custom identifier with Scope set to Object.&#x20;
{% endhint %}

### Execution Nodes

These nodes do something based on an Object input, such as modifying an Object.

* Set Object Position

## Known Objects

Below is a list of valid and invalid objects. Invalid Objects are types of entities that cannot be referenced at all through scripting.

| Valid                       | Invalid            |
| --------------------------- | ------------------ |
| All Objects Placed in Forge | Dead Players       |
| Thrown Grenades/Projectiles | Destroyed Vehicles |
| Players                     |                    |
