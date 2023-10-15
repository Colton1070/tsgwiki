---
description: >-
  The unofficial designations that this Wiki utilizes to refer to, and simplify,
  Nodes.
---

# Node Types

## Introduction

Node types are a way to organize nodes based on what they do. While there are nodes of various categories within Halo Infinite, _Node Types_, specifically designates nodes based on their characteristics.

## Overview

* [event-node.md](event-node.md "mention")(s)
  * Triggered by a game event, or custom event.
  * Can temporarily store and provide data via its output connection pins.
  * May accept data inputs which arm or configure the event.
* [execution-node.md](execution-node.md "mention")(s)
  * Triggered by an execution connection via it's input execution pin.
  * May also temporarily store and provide date via its output connection pins, as well as require or receive optional input data to successfully execute.
* [data-node](data-node/ "mention")(s)
  * Does not have any input [execution pins](../connection-pins/execution-pin.md). Performs an operation when an execution node it is related to is triggered. Data nodes send information forward and can be combined to create complex operations to prepare data for an execution node.
  * May feed into one or many execution nodes within the same event.
