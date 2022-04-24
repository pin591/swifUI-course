# How to create stacks using VStack and HStack

When we want more than one view on screen at a time you’ll usually want to tell SwiftUI how to arrange them, and that’s where stacks come in.

Stacks are the equivalent to UIStackView in UIKit 

Come in three forms: horizontal(HStack), vertical (VStack) and depth-based (ZStack),

## VStack

If we want to place elements vertically so our view elements are placed above each other

```swift
VStack {
    Text("SwiftUI")
    Text("rocks")
}
```

Vertical stack is placed by default at the center of the screen, with the labels also being centered and having some automatic space between them.

## HStacks

If we want to place our view elements placed side by side horizontally we use HStacks

```swift
HStack {
    Text("SwiftUI")
    Text("rocks")
}
```
