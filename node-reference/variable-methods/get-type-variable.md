---
description: >-
  A method that exists for many Variable Types which allows for the retrieval of
  a Variable's value.
---

# Get \[Type] Variable

## Definition

After being declared, variables can be retrieved via a variable type's "Get" method. The node will return the value of a variable matching the Identifier and Scope.

### Inputs

#### Identifier

Identifier is the custom string that is used to identify a variable. Identifier is set when the variable is declared.

#### Scope

Scope is the [Scope ](../scope/)of the Variable being retrieved.

#### Object

The Object input pin is only used when Scope is set to "Object". When the Object Scope is used, and a valid object is connected to the node, this node will return _that_ object's value. Read more about Object Scope here.

### Variable Types

List of variable types which support this type of Node.

* Get Boolean Variable
* Get Equipment Type Variable
* Get Grenade Type Variable
* Get Number Variable
* Get Object List Variable
* Get Object Variable
* Get String Variable
* Get Team Variable
* Get UI Message Variable
* Get Vector3 Variable
* Get Vehicle Type Variable
* Get Weapon Type Variable

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
