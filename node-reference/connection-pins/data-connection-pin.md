---
description: The data connection pin is used to link data from one node to another.
---

# Data Connection Pin

## Introduction

Data connection pins allow nodes to receive and provide data of one of the [Variable Types](../data-types/).

<details>

<summary>Input Pin</summary>

An input connection pin is used to receive data from another node.\
Some input connection pins do not have a corresponding node or Variable Type, rather - the node accepts input directly via it's Node Properties.

</details>

<details>

<summary>Output Pin</summary>

An output data connection pin, when connected to an input data connection pin on another node, will forward data for a given operation to that node.

May be connected to multiple [Execution ](../node-types/execution-node.md)and [Data ](../node-types/data-node/)nodes, can **not** be shared across [Event ](../node-types/event-node.md)nodes.

</details>

{% tabs %}
{% tab title="Examples" %}


<div>

<figure><img src="../../.gitbook/assets/Untitled.png" alt=""><figcaption><p>Above, the player is being received by the Print Player to Killfeed node from the On Player Mark Event.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ExecutionPinForEach.png" alt=""><figcaption><p>Get All Players provides an Object List of Players when the For Each Object executes - at game start in this circumstance. Nodes will always provide the most current version of data that they provide via the data connection pin.</p></figcaption></figure>

</div>
{% endtab %}
{% endtabs %}

#### See Also
