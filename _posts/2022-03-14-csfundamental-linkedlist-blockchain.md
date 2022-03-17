---
layout: post
title:  "CS Fundamentals of Cryptocurrency(1): Linkedlist and Blockchain"
date:   2022-03-14 17:15:30 -0500
categories: cryptoeconomy
---

Linked list is a data structure that contains a sequence of nodes such that each node contains an object and reference to the next object. It has two main types: singly linked list and doubly linked list.

1. Singly linked list

![Screenshot from 2022-03-17 16-33-47](/images/singlylinkedlist.png)

```python
class Node:
  def __init__(self,data):
    self.data=data
    self.next=None
```

2. Doubly linked list

![Screenshot from 2022-03-17 16-37-43](/images/doublylinkedlist.png)

```python
class Node:
  def __init__(self,data):
    self.data=data
    self.next=None
    self.prev=None
```

## Understand Blockchain from linked list

The blockchain is very similar to an ordered back-linked list of blocks of transactions in a crypto-economy system. It also has some differences.

Each block is a container made up of block size, block header, transaction counter, and transactions. It is identified by a hash, generated using the SHA256 cryptographic hash algorithm on the header of the block.

The main difference between a blockchain and a linked list is data in the blockchain can not be altered or erased.

## Pros and cons of linked list

For a linked list, insertion and deletion operation is cheap(O(1)). It's also a dynamic data structure with no memory wastage. This property indicates once a block has been created and verified, it can be added very swiftly to the blockchain. In addition, the length of the blockchain is limitless.

A search operation of a linked list is expensive, thus time to locate a data node in the list increases with the length of the list. Blockchain suppresses this weakness by maintaining a bunch of indices so that you can find blocks and transactions by hash.

## Exercises

1. Try reverse a linked list using an iterative method and a recursive method

```python
def reverse(head):
    if head is None:
        return head
    if head.next is None:
        return head
    node1 = reverse(head.next)
    head.next.next = head
    head.next = None
    return node1

def reverse(head):
    prev = None
    cur = head
    while cur:
        t = cur.next
        cur.next = prev
        prev = cur
        cur = t
    return prev
```

