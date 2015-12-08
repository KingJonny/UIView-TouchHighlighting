# UIView+TouchHighlighting
UIView+TouchHighlighting is a UIView category that provides a generic touch highlighting solution.
![Screenshot](https://github.com/mta452/UIView-TouchHighlighting/blob/master/SCREENSHOT.png)

## Usage
The category provides the following enum for highlighting a view.
```
NS_ENUM(NSInteger, MTHighlightingStyle) {
    MTHighlightingStyleNone,
    MTHighlightingStyleTransparentMask,
    MTHighlightingStyleLightBackground,
    MTHighlightingStyleSolidDarkOverlay,
    MTHighlightingStyleHollowDarkOverlay,
}
```

* `MTHighlightingStyleTransparentMask` introduces a transparent mask layer on touch.

* `MTHighlightingStyleLightBackground` introduces a light transparent background on touch.

* `MTHighlightingStyleSolidDarkOverlay` introduces a rectangular dark overlay layer on touch.

* `MTHighlightingStyleHollowDarkOverlay` introduces a dark overlay layer masked with view contents on touch.


Touch highlighting can be enabled on any view by setting `touchHighlightingStyle` property to desired value as follows.
```
  buttonView.touchHighlightingStyle = MTHighlightingStyleTransparentMask;
```


To disable touch highlighting, set `touchHighlightingStyle` property to `MTHighlightingStyleNone` as follows.
```
  buttonView.touchHighlightingStyle = MTHighlightingStyleNone;
```

## License
```
Copyright (C) 2015 Muhammad Tayyab Akram

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

  http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```