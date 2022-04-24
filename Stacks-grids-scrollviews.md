# How to create stacks using VStack and HStack

When we want more than one view on screen at a time you’ll usually want to tell SwiftUI how to arrange them, and that’s where stacks come in.

Stacks are the equivalent to **UIStackView** in UIKit 

Come in three forms: horizontal **HStack**, vertical **VStack** and depth-based **ZStack**,

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

# How to customize stack layouts with spacing: (vertical space)

You can add spacing inside your SwiftUI stacks by providing a value in the initializer, like this:

```swift
VStack(spacing: 50) {
    Text("SwiftUI")
    Text("rocks")
}
```

We can create dividers between items so that SwiftUI makes a small visual distinction between each item in the stack, like this:

```swift
VStack {
    Text("SwiftUI")
    Divider()
    Text("rocks")
}
```

# How to customize stack layouts with aligment (horitzontal space)

By default, items in your stacks are aligned centrally. In the case of HStack that means items are aligned to be vertically in the middle. **so if you have two text views of different heights they would both be aligned to their vertical center.**

For VStack that means items are aligned to be horizontally in the middle, so if you have two text views of different lengths they would both be aligned to their horizontal center.

we can adjust this by providing a value for the alignment paramenter in the initializer of the stack, like this:

```swift
VStack(alignment: .leading) {
    Text("SwiftUI")
    Text("rocks")
} 
```

You can of course use both alignment and spacing at the same time, like this:

```swift
VStack(alignment: .leading, spacing: 20) {
    Text("SwiftUI")
    Text("rocks")
}
```
That will align both text views horizontally to the leading edge (that’s left for left to right languages), and place 20 points of vertical space between them.

# How to force views to one side inside a stack using Spacer




