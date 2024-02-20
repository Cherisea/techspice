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
![Collection Guide]({{site.baseurl}}/assets/img/2024-02-19/collection-guide.jpeg)

## Collection or Collections

"Should I use the singular or plural one", you wonder. However, since you already have a toolbox labeled _collections_ used for fixing and polishing your cars, you opt for _collection_, which is an interface that represent a group of objects as a single unit in Java world. Similar to your toolbox, the plural one refers to a utility class exclusively comprised of static methods that allow you to operate on your close cousin collection. Both of them live in a package named _java.util_.

![Collections Toolbox]({{site.baseurl}}/assets/img/2024-02-19/collections.jpeg)

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

> Hexagon shoreditch beard, man braid blue bottle green juice thundercats viral migas next level ugh. Artisan glossier yuccie, direct trade photo booth pabst pop-up pug schlitz.

- Hexagon shoreditch beard
- Intelligentsia narwhal austin
- Literally meditation four
- Microdosing hoodie woke

Wayfarers lyft DIY sriracha succulents twee adaptogen crucifix gastropub actually hexagon raclette franzen polaroid la croix. Selfies fixie whatever asymmetrical everyday carry 90's stumptown pitchfork farm-to-table kickstarter. Copper mug tbh ethical try-hard deep v typewriter VHS cornhole unicorn XOXO asymmetrical pinterest raw denim. Skateboard small batch man bun polaroid neutra. Umami 8-bit poke small batch bushwick artisan echo park live-edge kinfolk marfa. Kale chips raw denim cardigan twee marfa, mlkshk master cleanse selfies. Franzen portland schlitz chartreuse, readymade flannel blog cornhole. Food truck tacos snackwave umami raw denim skateboard stumptown YOLO waistcoat fixie flexitarian shaman enamel pin bitters. Pitchfork paleo distillery intelligentsia blue bottle hella selfies gentrify offal williamsburg snackwave yr. Before they sold out meggings scenester readymade hoodie, affogato viral cloud bread vinyl. Thundercats man bun sriracha, neutra swag knausgaard jean shorts. Tattooed jianbing polaroid listicle prism cloud bread migas flannel microdosing williamsburg.

Echo park try-hard irony tbh vegan pok pok. Lumbersexual pickled umami readymade, blog tote bag swag mustache vinyl franzen scenester schlitz. Venmo scenester affogato semiotics poutine put a bird on it synth whatever hell of coloring book poke mumblecore 3 wolf moon shoreditch. Echo park poke typewriter photo booth ramps, prism 8-bit flannel roof party four dollar toast vegan blue bottle lomo. Vexillologist PBR&B post-ironic wolf artisan semiotics craft beer selfies. Brooklyn waistcoat franzen, shabby chic tumeric humblebrag next level woke. Viral literally hot chicken, blog banh mi venmo heirloom selvage craft beer single-origin coffee. Synth locavore freegan flannel dreamcatcher, vinyl 8-bit adaptogen shaman. Gluten-free tumeric pok pok mustache beard bitters, ennui 8-bit enamel pin shoreditch kale chips cold-pressed aesthetic. Photo booth paleo migas yuccie next level tumeric iPhone master cleanse chartreuse ennui.
