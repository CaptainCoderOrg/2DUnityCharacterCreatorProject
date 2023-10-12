---
title: "Part 12: Challenges"
layout: page
nav_order: 12
---

# Part 12: Challenges
{: .no_toc }


<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

Throughout this project, you have explored the basics of the Unity Canvas
system. This is less than 1% of everything Unity has to offer. Unfortunately, a
single project or guide will never be able to teach you everything that the
engine has to offer. However, there are thousands of fantastic resources
available for you to learn from. It is now your turn to explore a topic of your
choosing to expand upon this project. Below are several challenges that you can
choose from. Or, if you're feeling ambitious, come up with one of your own!

# Resources You Could Use (All from OpenGameArt.org)
* Pixel Art Food Builder Icons: [LINK](https://opengameart.org/content/lpc-meals)
* Adventure Game Equipment Sprites: [LINK](https://opengameart.org/content/armor-icons-by-equipment-slot)
* Fantasy Icons: [LINK](https://opengameart.org/content/fantasy-icon-pack-by-ravenmore-0)
* Parallax Background: [LINK](https://opengameart.org/content/pixel-art-parallax-background)
* Underground Background: [LINK](https://opengameart.org/content/underground-sidescroller-background)
* Space Background: [LINK](https://opengameart.org/content/space-background-3)

# Challenges

## Add Background Music (Easy)

Research how to add an Audio Source to your scene to play a music file. When the
`Weapon Shop` or `Armor Shop` are open, add an **Event Listener** that changes
the music.

You an use any music you'd like but here are a few that I have written that you
can use: [LINK](https://opengameart.org/art-search?keys=jocolloman)

## Add Sound Effects (Easy)

Find several sound effects that can be played when a weapon or Armor item is
selected. For example, each weapon could have a different sound:

* The stick makes a "thud" sound
* The sword makes a "schwing" sounds
* The Chain armor makes a "chunk" sound

Right click and add an "Audio > Audio Source" to your Scene. This will allow you
to play audio. Play with the options and see what you can learn!

This RPG Sound Pack is an excellent option to get started:
[LINK](https://opengameart.org/content/rpg-sound-pack)

## Add Text Information Bout Each Item (Medium)

Add text elements to your scene to display the name, description, and price of each item.

* Create a new Canvas for your text elements (they shouldn't disappear when you switch shops)
* Add 3 text elements to the new canvas
* Position them in a "pleasing" way on the screen.
* Add the appropriate Event Listeners to each buttons OnClick event.

Demo of a project with this feature: [LINK](https://jcollard.github.io/CharacterCreatorDemo/)

## Add a "Magic Shop" Using Particle Effects (Medium)

Research how to use the Particle Effect system built into Unity to make a "Magic Shop".

* Add a Magic Game Object to your Player Game Object
* Inside of the Magic Game Object, add an Effects > Particle System
* Rename the Particle System something like "Blue Magic"
* Play with the Particle System features in the Inspector
* Make several (at least 3) different "Magic" options
* Create a Magic Shop canvas with buttons which call the SetActive option appropriately for each of your "Magic" effects.

Demo of a project with this feature: [LINK](https://jcollard.github.io/CharacterCreatorDemo/)

## Monster Selector (Medium)


The sprites you're using for this project come from a game that has additional
assets. Make a second project using those assets. A "Monster Selector" would be
great! But, you can suggest another project of your own design.

Enemies: [LINK](https://github.com/ChadwickCSP/CharacterCreator/blob/main/04_AdvancedFeatures/Files/enemies.zip)

The idea here is to use the enemy images to create a project similar to this one
which shows the enemy image and displays a little information about them.

## Character Randomizer (Hard)

Research how to use the Random class to generate random numbers. Then, using the
randomly generated number, call a specific buttons OnClick method.

* Create a public List<UnityEngine.UI.Button> WeaponButtons; in your PlayerController
* Write a method public void SetRandomWeapon()
* Use the Random class to generate a number between 0 and WeaponButtons.Count.
* Select the button from the list using generated number (e.g. WeaponButtons[0])
* Call the button's onClick.Invoke() method (e.g. WeaponButtons.[0].onClick.Invoke())
* Create a new button in your Weapon Shop called Random Weapon
* Update the Random Weapon button to call SetRandomWeapon()
* Repeat the above s
* Bonus: Add a Random Character button that calls both methods.

{% include Links.md %}