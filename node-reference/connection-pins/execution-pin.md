---
description: The execution pin is used to attach two execution nodes together.
---

# Execution Pin

## Introduction

Execution Pins define the flow of logic within a Node Graph. Scripts execute in a pattern that is "Left to right" assuming scripts are ordered horizontally. Each node within the chain is connected sequentially using the execution pins.\
\
Execution pins are usually represented by diamonds, except in cases where a Node provides multiple output execution pins.

<details>

<summary>Input Pin</summary>

An input execution pin, when connected to an output execution pin, will place the node it belongs to within the execution chain. This node will trigger sequentially on the completion of the execution node before it. If left disconnected, nothing will trigger this execution node.\
\
Events do not carry input execution pins, due to the nature of their execution being tied to a timer or in game event.

</details>

<details>

<summary>Output Pin</summary>

An output execution pin, when connected to an input execution pin on another node, will trigger the execution node this pin is connected to, after this execution node has completed.\
\
Certain nodes, like Branch



</details>

{% tabs %}
{% tab title="Examples" %}


<div>

<figure><img src="../../.gitbook/assets/Untitled.png" alt=""><figcaption><p>Above, an event's output execution pin is connected to a node input execution pin.</p></figcaption></figure>

 

<figure><img src="../../.gitbook/assets/ExecutionPinForEach.png" alt=""><figcaption><p>Not all execution pins may be represented by diamonds. Due to engine limitations, some execution pins are circles instead. You would still connect the On Completion to the rest of the execution chain, and connect Execute Per Object to an isolated chain you would like to loop for each of the objects in the input object list.</p></figcaption></figure>

</div>
{% endtab %}
{% endtabs %}

#### See Also
