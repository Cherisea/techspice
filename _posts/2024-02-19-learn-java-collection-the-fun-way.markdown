---
layout: post
title: Learn Java Collection The Fun Way
date: 2024-02-19 16:44:20 +0300
description: explore the use cases of a wide array of Java collection
img: car-collection.jpg
fig-caption: a collection of toy cars
tags: [Java, Collection]
---

Imagine that you're an aficionado of cars who owns a collection of car toys in your home (I know it would be wonderful if they are real). In fact, there are so many of them that you don't even know how many you have and where they come from. So you decide to categorize them by a certain criterion using Java, but several issues immediately crop up.

- Should you assign a unique label to each of your cars and store them as key, value pairs?
- Do you have cars that're exactly the same?
- Do you prefer fast retrieval or preditable order of iteration?
- Would you like to preserve the order in which your cars are inserted?
- Do you often need to add new cars to or remove existing cars from your collection?
- Do you want to ensure the first car in is also the first car out?

After some research, you found this general guide.
![Collection Guide]({{site.baseurl}}/assets/img/2024-02-19/collection-guide.png)

It looks overwhelming, so you want to dig a little deeper.

## **Collection or Collections**

"Should I use the singular or plural one", you wonder. However, since you already have a toolbox labeled **_collections_** used for fixing and polishing your cars, you opt for **_collection_**, which is an interface that represent a group of objects as a single unit in Java world. Similar to your toolbox, the plural one refers to a utility class exclusively comprised of static methods that allow you to operate on your close cousin collection. Both of them live in a package named **_java.util_**.

![Collections Toolbox]({{site.baseurl}}/assets/img/2024-02-19/collections.jpeg)

> [!TIP] > **Collection** is the root interface of Java collection framework, while **Collections** is a utility class consisting of static methods that operate on specific implementations of Collection.

## **List, Set, Queue or Map**

Having picked a name for your valuable assortment of cars, you run into another problem, "What kind of collection should I use to sort them? After all, collection is an interface that doesn't offer any specific guidance on how I should arrange my cars." Maybe employing a list interface if you have two Porsche 911 that are exactly the same?

![List]({{site.baseurl}}/assets/img/2024-02-19/list.jpeg)

### ArrayList

You don't want to hear your mom complaining again about your cars strewn in the kitchen. Plus, she "accidentically" broke one of your favorite Farrari on a horrrible morning (you know she did that as a warning, although she claimed it was an accident). So, you resolve to allocate an area in your room exclusively for your cars. But what if you run out of space in that area when you bring in more cars later on?

In that case, you could increase its size by 50%. But you would have to copy all cars and move them to their new place. The extra workload scares you off, "Maybe not as an arraylist".

### LinkedList

Instead of a fixed-size ArrayList, you come up with an ingenious idea, "Wouldn't it be wonderful if I put my cars anywhere I want and put a sticker on them that indicates its previous and next cars in the list?"

"But then I would have to trace from the front or rear every time I want to find a car. What if the car I look for sits in the middle?" You can't even bear that thought.

### Vector

Compared to an ArrayList, a vector allows you to double your designated area by default every time you need to resize. Besides, if you ask your friend Tom to work on this together, his work will be synchronized on your end as well. Therefore, you never have to worry about being left out of the loop. "I'll make this plan A."

![Set]({{site.baseurl}}/assets/img/2024-02-19/set.jpeg)

After much deliberation, you realize that spending extra bucks on the same models is just not worth it. You want a collection that covers as diverse range of cars as possible. But which set is the most fittig choice?

### TreeSet

Treeset sorts your cars using natural ordering or a custom comparator at creation time, giving you the opportunity to show off your cars to friends by their price or year of production.

"My friends are gonna be so jealous of me", you couldn't help laughing at the thought of that. Then, the grin on your face suddenly freezes, "It would take me forever to find a specific car if my friend ever requests." You decide to ditch this idea cause you don't want to embrass yourself in front of your friends.

### HashSet

"This one allows me to readily retrieve a car my friends ask for, but it can't guarantee that my cars are sorted. What's the fun of that?" You seems to run into a pickle until another option grabs your attention.

### LinkedHashSet

While maintaining the order in which your cars are inserted into it, LinkedHashSet isn't capable of offering the same sorting functionality as that of TreeSet. You could fetch your cars in the same order they are added to your collection and locate any one fast enough to amaze your friends, but you can't be sure they are sorted by a certain standard. "Guess I'll just keep looking", you heaved a sigh.

> [!TIP] > **LinkedHashSet** is an implementation of set interface with **Hash table** and **linked list**, ensuring that iteration order is consistant with its insertion order. It basically sits somewhere between **HashSet** and **TreeSet** in terms of performance and sorting.

![Queue]({{site.baseurl}}/assets/img/2024-02-19/queue.jpeg)

After a day's work, you feel like you have got nowhere on your car collection sorting project. Out of deperation, you reached out to your friend Tom for help, tasking him with passing cars to you while you figure out how they should be sorted. To ensure fairness, you want the cars that are handed down to you first to be processed first.

### PriorityQueue

While this one enables you to sort your cars based on natural ordering or a coustom order defined by a comparator, it doesn't preserve the original insertion order. "That's not fair", you thought to yourself.

### LinkedList

By contrast, ListedList maintains the order in which cars are inserted, but you can't sort them. It seems like there is no perfect collection to sort your car collection.

![Map]({{site.baseurl}}/assets/img/2024-02-19/map.jpeg)

"Maybe I should just leave them the way they are. This is no suitable solutions to this." You say to Tom, shrugging your shoulders.

"Isn't there another type of collection you haven't tried yet? Something called map?" Tom remind you.

"But it doesn't extend from the collection interface, which means it's an outsider. I don't think collection would be happy with that." You caution.

"How can you say that? Map is still considered part of collection. It's family." Tom retort, feeling indignant for map.

"Okay, but that means it shares all the characteristics of other members. It's either fast, sorted or consistant with insertion order, but you can never get all of them at once. Not to mention the synchronization issue. Why don't we just have a great time and forget about sorting?"

"Yeah, I guess you're right." Tom isn't a fan of drudgery, so he happily complies.
