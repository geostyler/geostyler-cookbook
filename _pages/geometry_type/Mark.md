---
title: Mark
author: Krishna Lodha
date: 2022-06-07
category: geometry type
layout: post
---



# **Symbolizer Type**

`Mark` represents the visualization of `Point` data.

Point is a simple geometry type, even though it has position as a coordinates attached to it, we can certainly style it using various ways using  [Geostyler](https://geostyler.org/) 

# **UI of styler**

Once data is loaded, [Geostyler](https://geostyler.org/) automatically detects the geometry type and tries to set it up, click in column of *paint bucket*

`Mark` supports various properties to create perfect styling for Points. 
![Mark Symbolizer]( ../../images/mark_sym.png "Mark Symbolizer")

For each change in the properties, you can see preview
![Mark preview]( ../../images/preview_mark.png "Mark preview")



## Symbols

`Mark` supports various symbol lists right out of the box such as `circle`,`square`,`triangle`,`star`,`cross`,`x` , it also provides shapes such as `backslash` , `carrow`, `dot`, `horline`, `oarrow`, `plus`, `slash`, `times`, `vertline`.

Once you select these, you can check the preview to see how it looks

![Mark cross]( ../../images/mark_cross.png "Mark cross")

![Mark arrow]( ../../images/mark_arrow.png "Mark arrow")


## Radius

`Radius` is the general term use to define the size of the `Mark` , you can set it up as per convenience

## Fill-color

`Fill-color` allows user to select colour for filling the `Mark` . You can select colour by following methods

- Selection from Colour Panel
- Hex ID
- RGB
- Selection from predefined colors

![Mark fill_color]( ../../images/mark_fill_color.png "Mark fill_color")

## Opacity

`Opacity` defines the transparency of the `Mark`, values can be set between **0 - 1**, where 0 means transparent and 1 means opaque

![Mark opacity]( ../../images/mark_opacity.png "Mark opacity")


## Fill-Opacity

Using `Fill-opacity` user can specify the transparency of colour used in `Fill-color` , User can create combination of `Fill-opacity` and `stroke-opacity`

<aside>
🚀 Note : This might not reflect properly in preview, but developers are working on it, and will be resolved soon

</aside>

## Stroke-Colour

This property defines the color of the border of the `Mark`. Selection of Colour works the same way as `Fill-color`

## Stroke-Opacity

This property is used to define transparency of the border. User can set different opacity for `fill` and `stroke` .

Values can be set between **0 - 1**, where 0 means transparent and 1 means opaque


## Stroke-Width

`Stroke-Width` is used to set thickness of the border

## Rotation

Using `Rotation`, user can rotate the symbol at given value in degree