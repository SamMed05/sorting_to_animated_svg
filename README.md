# Sorting Algorithm Visualizer & Compact Animated SVG Exporter

An interactive web-based sorting algorithm visualizer that compiles algorithm execution traces into **standalone animated SVGs** suitable for embedding anywhere.

* 8 core sorting algorithms, including Quick, Merge, Heap, Radix, and standard comparison sorts
* Dynamic visuals featuring recursion range highlighting, swap/scan markers, and adaptive theme support using `currentColor` and `prefers-color-scheme`
* Interactive play/pause toggle embedded directly into the generated SVG
* Zero external dependencies (built with pure HTML5, vanilla JS, CSS, and native SVG SMIL)

### Demo/Example

This is an example of an animated and playable/stoppable merge sort visualization the generator can output:

![Merge Sort Animation](merge_animated.svg)

> Note: GitHub does not support embedding raw, inline SVG XML code directly inside a markdown file for security and cross-site scripting (XSS) prevention. If you are unable to play/pause the animation with the button, download the SVG to try it!

### SVG Embedding

The exported SVGs are fully self-contained vector files.

For full interactivity (the embedded play/pause toggle), embed via `<object>` or inline:

```html
<!-- Interactive (play/pause toggle works) -->
<object type="image/svg+xml" data="merge_animated.svg"></object>

<!-- Static looped graphic (Markdown / standard img) -->
<img src="merge_animated.svg" alt="Merge Sort Animation" />
```

### Further developments

While no major new features are planned, ideally a complete version of this tool would make more advanced animations, arrows and ![intermediate visuals](https://commons.wikimedia.org/wiki/File:Sorting_heapsort_anim.gif) better specialized for each algorithm and more useful to understand the sorting process, like the popular sorting algorithm GIFs present on Wikipedia, created with Ruby 1.8.4 and RMagick by user [RolandH](https://de.wikipedia.org/wiki/Benutzer:RolandH):

[![Sorting quicksort anim](https://upload.wikimedia.org/wikipedia/commons/6/6a/Sorting_quicksort_anim.gif?utm_source=commons.wikimedia.org&utm_campaign=imageinfo&utm_content=original)](https://commons.wikimedia.org/wiki/File:Sorting_quicksort_anim.gif#/media/File:Sorting_quicksort_anim.gif)

By [en:User:RolandH](https://en.wikipedia.org/wiki/User:RolandH), [CC BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/), [Link](https://commons.wikimedia.org/w/index.php?curid=1965827)
