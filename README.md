

##  Package
A CrossScroll is a flutter Package that permits it’s child views to be scrolled vertically and Horizontally. This is important because in many cases you need content to be scrolled on both side. 











[![Gitter](https://badges.gitter.im/METRA-IT/community.svg)](https://gitter.im/METRA-IT/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
<a href="https://github.com/Mehrankhan-METRA-RGB/cross_scroll/actions">
<img src="https://github.com/EdsonBueno/infinite_scroll_pagination/workflows/build/badge.svg">
</a>
<a href="https://github.com/Mehrankhan-METRA-RGB/cross_scroll">
<img src="https://img.shields.io/badge/platform-flutter-ff69b4.svg" >
</a>

---





### List of features
- The vertical scrollbar wil never  hides when the scrolling on horizontal axis and vice versa. The scrollBar never hides with scrolling on any directions.
- Support track onClick scrolls.
- Support thumb Drag scrolls.
- Support All feature `SingleChildScrollView` have.







## Tested Platform

#### WEB
- MicroSoft Edge

![cross_scroll web test](https://user-images.githubusercontent.com/73336909/149651423-d1dc936f-cfc0-4581-bb79-19e1fc4ec533.gif)




















#### Windows
- Windows 10

![cross_scroll window test](https://user-images.githubusercontent.com/73336909/149651492-2ce542a7-7343-4651-81b1-d3eccf3f9bda.gif)












## Getting started



## CrossScroll
```dart
CrossScroll(verticalBar: sc,
      horizontalBar:sc ,
      child: Column(
        children: [
          for (var i = 1; i < 11; i++)
            Row(
              children: [
                for (var i = 1; i < 11; i++)
                  Container(
                    margin:const EdgeInsets.all(2),
                    width: MediaQuery.of(context).size.width/2,
                    height: MediaQuery.of(context).size.height/2,
                    color: colors[random.nextInt(13).round().toInt()],
                  ),
              ],
            )

        ],
      ),
    )

```




#### CrossScrollBar
```dart
final CrossScrollBar _crossScrollBar= const CrossScrollBar(
  isAlwaysShown:true,
  hoverThickness: 8,
  thickness :8,
  radius : Radius.elliptical(8, 8),
  showTrackOnHover: true,
  trackVisibility: false,
);
```












#### CrossScrollStyle
```dart
 final CrossScrollStyle _crossScrollStyle =  CrossScrollStyle(
    physics: BouncingScrollPhysics(),
    clipBehavior:Clip.hardEdge,
    dragStartBehavior: DragStartBehavior.start,
    keyboardDismissBehavior: ScrollViewKeyboardDismissBehavior.manual,
    reverse: false,
    padding:const EdgeInsets.symmetric(vertical: 2),
  );

```














## Additional information

TODO: Tell users more about the package: where to find more information, how to 
contribute to the package, how to file issues, what response they can expect 
from the package authors, and more.
