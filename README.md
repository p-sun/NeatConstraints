# NeatConstraints
An clean way to create `NSLayoutConstraints` programmatically! Easier to use than the native API, and easier to skim and debug than most storyboards since you don't need to click through many subviews to see all the constraints. Heavily modified from [TinyConstraints](https://github.com/roberthein/TinyConstraints).

## How to Install
- Drag the `NeatConstraints` folder to your project. Done.

## Why create constraints programmatically instead of with storyboards?

- It's often easier to debug than storyboards because you can read all the constraints at once, instead of clicking through many views on the storyboards. It's easy to miss details on storyboards, especially if you set priorities.

- You can write your own library! (i.e. constrainViewToCustomNavigationBar)

- It makes you create other views, segues, and classes programmatically too. This makes it easier to see what settings you have changed from the default (i.e. isEnabled, isHidden) than skimming through the property inspector on storyboards.

- Programmatic creation of all things means you can easily modularize all things instead of setting them in the storyboard manually! Like text font and color!

- You can share views created programically easier than than you can share nibs. Sharing is caring. Love yourself -- reuse cool stuff from previous projects, [like cool custom menu with custom buttons](https://github.com/p-sun/Rounded-Bordered-Button-Menus).

- Easy read the difference in code reviews.

- "Storyboards are not modular. Nibs are annoying to use. It's really the best of bad options" - @CarlNathan

## How about small nibs?

- That being said, nibs are fine for constraining tiny views. [The NibView protocol](https://github.com/p-sun/NeatConstraints/blob/master/NeatConstraintsDemo/NeatConstraintsDemo/NeatConstraints/NibView.swift) could make your life easier because now you can go `let view: CustomView = CustomView.instanceFromNib()`

## ViewController Demo
- See how it's used in [ViewController.swift](https://github.com/p-sun/NeatConstraints/blob/master/NeatConstraintsDemo/NeatConstraintsDemo/ViewController.swift).
- Type `.constrain` on any `UIView` and let autocomplete tell you what's available. Make sure to add your subviews to your view hierachy before you constrain it.

![demo][demo]

[demo]: https://github.com/p-sun/NeatConstraints/blob/master/demo.gif
