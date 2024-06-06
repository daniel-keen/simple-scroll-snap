<h1 align="middle">Simple Scroll-Snap (Fork) by Daniel Keen</h1>
<p align="middle">This is a fork of the original Simple Scroll-Snap library made by <a href="https://github.com/daniellochner/simple-scroll-snap/commits?author=daniellochner">Daniel Lochner</a>.</p>

## Installation
Install via UPM:
```https://github.com/daniel-keen/simple-scroll-snap.git```  

## Forked Features:
- Install via Unity Package Manager
- Add items without instantiating them under the hood, like so:
```
private MyPrefabComponent MyPrefab;

void Test(object someData)
{
    var item = Instantiate(MyPrefab, scrollSnap.Content);
    item.Initialize(someData);  // You can do something with your object.
    scrollSnap.AddToBack(item.gameObject);
}
```

## Features:
- Fixed (Horizontal/Vertical) or Free movement system.
- Optional Automatic Layout system.
- Optional Infinite Scrolling system.
- Navigate between panels using Swipe Gestures, a Pagination and/or Next and Previous buttons.
- Easily implement Transition Effects (adjusting panels' scale, rotation, opacity etc.) using functions with respect to displacement from the center.
- Change to snap to the Nearest, Previous or Next panel.
- Define Threshold Swipe and Snap Speeds to best fit your requirements.
- Assign methods to be invoked while a panel is being selected, is selected, is being changed or has changed.
- Dynamically add/remove panels during runtime.
- ... and much more!

## Included:
- Five example projects (macOS Finder (File Explorer), iOS Home Screen, Slot Machine, Pinned Map, Dynamic Content)
- Ready-to-use prefabs (Scroll-Snap, Pagination)
- In-depth offline documentation

## Help:
In the event you are unable to find the information you are looking for or have found a bug, please raise an issue here or post a question in the [Discord server](https://discord.gg/sJysbdu).
