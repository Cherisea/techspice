---
layout: post
title: Learn Java Collection The Fun Way
date: 2024-02-19 16:44:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: car-collection.jpg
fig-caption: a collection of toy cars
tags: [Holidays, Hawaii]
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

## Collection or Collections

"Should I use the singular or plural one", you wonder. However, since you already have a toolbox labeled **_collections_** used for fixing and polishing your cars, you opt for **_collection_**, which is an interface that represent a group of objects as a single unit in Java world. Similar to your toolbox, the plural one refers to a utility class exclusively comprised of static methods that allow you to operate on your close cousin collection. Both of them live in a package named **_java.util_**.

![Collections Toolbox]({{site.baseurl}}/assets/img/2024-02-19/collections.jpeg)

> [!TIP]
> Collection is the root interface of Java collection framework, while Collections is a utility class consisting of static methods that operate on specific implementations of Collection.

## List, Set, Queue or Map

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
