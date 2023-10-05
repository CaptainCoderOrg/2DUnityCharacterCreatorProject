---
title: "Part 10: Adding Text"
layout: page
nav_order: 10
---

# Part 10: Adding Text
{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

## Creating an Item Description Dialog

Each item that can be selected from your menus will have 3 properties:

1. A Name
2. A Price
3. A Description

## Create a Container for the Selected Item Info

To display this information, you can create a container to hold 3 `Text` `GameObjects`:

Within your `Canvas` element, add a new `GameObject` to be the container.

![Create Container](../imgs/10/00-create-container.png)

Rename the container to reflect that it will display information about the
selected item. In this guide, it will be referred to as `Selected Item Info`.

![Selected Item Info](../imgs/10/01-selected-item-info.png)

## Adding a Text GameObject to the Selected Item Info Container

1. Right click on the `Selected Item Info` container to create a child component
2. Select `UI` > `Text - TextMeshPro`

![Create Text](../imgs/10/02-create-text-labels.png)

3. Rename the `GameObject` to reflect that this text will be the name of the item. In this guide, it will be referred to as `Item Name (Text)`.

![Item Name Text](../imgs/10/03-item-name.png)

## TextMeshPro - Text (UI) Component Properties

1. Select the `Item Name (Text)` `GameObject` in the `Hierarchy` tab
2. In the `Inspector` tab, find the `TextMeshPro - Text (UI)` component (you may have to scroll down)

![Find Component](../imgs/10/04-find-component.png)

The `TextMeshPro - Text (UI)` component provides properties you can modified to
change the way text is displayed on the screen. You may recall that your button
`GameObject`s each have one nested inside.

1. Change the displayed text to say be *Item Name*
2. Adjust the `Font Style` *Bold* by clicking the `B` in the `Main Settings`
3. Adjust the `Font Size` to be `64`

![Item Name Style](../imgs/10/05-item-name-style.png)

## Challenge: Add 2 More Text GameObjects

Remember that each item will have 3 properties: Name, Price, and Description

1. Add 2 more text game objects as children of the `Select Item Info` GameObject
   * One for `Item Price (Text)` 
   * Another for `Item Description (Text)`
2. Use a `Vertical Layout Group` to automagically size and place the labels in a
   way you find pleasing. 
   * **Optionally**: You may arrange them manually or using another layout manager of your choosing.
3. Adjust the styling of each of your text `GameObject`s to your liking.
4. If necessary, update the position of your armor and weapon buttons to fit nicely with your text.

When you're finished, your `Hierarchy` and `Game` view should look similar to this:

![Challenge Complete](../imgs/10/06-challenge-complete.png)

## What's Next?

<!-- In [Part 11: Changing Text]({% link pages/11-changing-text.md %}), you will update your buttons to modify the text  -->

{% include Links.md %}