# Sorting Algorithm Visualizer & Compact Animated SVG Exporter

An interactive web-based sorting algorithm visualizer that compiles algorithm execution traces into **standalone animated SVGs** suitable for embedding anywhere.

---

## Features

- **8 Core Sorting Algorithms**:
  - Quick Sort (Hoare & Lomuto partition variants)
  - Merge Sort
  - Heap Sort
  - Radix Sort (LSD)
  - Insertion Sort, Selection Sort, Bubble Sort
- **Visuals**:
  - Dynamic recursion range shading with faded out-of-scope elements.
  - Horizontal reference guidelines for partition pivot values.
  - Markers for scans, swaps, and comparisons.
  - Adaptive `currentColor` bars that automatically match dark or light backgrounds.
  - Transparent SVG canvas with a subtle semi-transparent border.
- **Interactive Pause/Play Toggle**:
  - Each exported SVG includes an embedded play/pause button (powered by native SMIL animation controls).
- **SVG Size Optimization**:
  - Run-length keyframe compaction strips redundant intermediate states.
  - Omission of static attributes and zero frame-bloat loop pauses.
  - Yields standalone vectors often **80%+ smaller** (~30–45 KB) than naive SMIL recordings.
- **Zero Dependencies**: Pure HTML5, vanilla JavaScript, CSS, and native SVG SMIL.

## Demo/Example

This is an example of an animated and playable/stoppable merge sort visualization the generator can output:

![merge animated](merge_animated.svg)

## SVG Embedding

The exported SVGs are fully self-contained vector files.

For full interactivity (the embedded play/pause toggle), embed via `<object>` or inline:

```html
<!-- Interactive (play/pause toggle works) -->
<object type="image/svg+xml" data="quick_sort_animated.svg"></object>

<!-- Static looped graphic (Markdown / standard img) -->
<img src="quick_sort_animated.svg" alt="Quick Sort Animation" />
```

## Further developments

While no major new features are planned, ideally a complete version of this tool would make more advanced animations, arrows and ![intermediate visuals](https://commons.wikimedia.org/wiki/File:Sorting_heapsort_anim.gif) better specialized for each algorithm and more useful to understand the sorting process, like the popular sorting algorithm GIFs present on Wikipedia, created with Ruby 1.8.4 and RMagick by user [RolandH](https://de.wikipedia.org/wiki/Benutzer:RolandH):

[![Sorting quicksort anim](https://upload.wikimedia.org/wikipedia/commons/6/6a/Sorting_quicksort_anim.gif?utm_source=commons.wikimedia.org&utm_campaign=imageinfo&utm_content=original)](https://commons.wikimedia.org/wiki/File:Sorting_quicksort_anim.gif#/media/File:Sorting_quicksort_anim.gif)

By [en:User:RolandH](https://en.wikipedia.org/wiki/User:RolandH), [CC BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/), [Link](https://commons.wikimedia.org/w/index.php?curid=1965827)
