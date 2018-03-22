# NeatConstraints
An clean way to create `NSLayoutConstraints` programmatically! Easier to use than the native API, and easier to skim and debug than most storyboards since you don't need to click through many subviews to see all the constraints. Heavily modified from [TinyConstraints](https://github.com/roberthein/TinyConstraints).

## How to Install
- Drag the `NeatConstraints` folder to your project. Done.

## Why create constraints programmatically?

- It's often easier to debug than storyboards because you can read all the constraints at once, instead of clicking through many views on the storyboards. It's easy to miss details on storyboards, especially if you set priorities.

- You can write your own library! (i.e. constrainViewToCustomNavigationBar)

- It makes you create other views, segues, and classes programmatically too. This makes it easier to see what settings you have changed from the default (i.e. isEnabled, isHidden) than skimming through the property inspector on storyboards.

- Programmatic creation of all things means you can easily modularize all things instead of setting them in the storyboard manually! Like text font and color!

- "Storyboards are not modular. Nibs are annoying to use. It's really the best of bad options" - @CarlNathan

## ViewController Demo
- See how it's used in [ViewController.swift](https://github.com/p-sun/NeatConstraints/blob/master/NeatConstraintsDemo/NeatConstraintsDemo/ViewController.swift).
- Type `.constrain` on any `UIView` and let autocomplete tell you what's available. Make sure to add your subviews to your view hierachy before you constrain it.

![demo][demo]

[demo]: https://github.com/p-sun/NeatConstraints/blob/master/demo.gif
