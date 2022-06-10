---
title: Filter
author: Krishna Lodha
date: 2022-06-07
category: functions
layout: post
---


# Filtering

Filtering allows users to create conditions based on _attributes_ available in the data. Depending on the _data type_ of the _attribute_ (e.g. number, boolean, string, etc. ) users can select operators and combine it with the _attributes_ available in the data.

Users can also add, remove, and convert one filter types into others using the UI.
![change_filter]( ../images/change_filter.png "change_filter")


# Comparison Filter (Default)

Comparison filtering involves comparing attributes with some value and only getting results out of it for which the comparison evaluates to true.

e.g. For given data we’ll check that all `pop_min` is less than 500.

![Basic filter]( ../images/basic_filter.png "Basic filter")

Here users select `attribute name` next to attribute name [Geostyler](https://geostyler.org/) automatically adds the `data type` and finally users can give input values. 

- For numeric data, operators such as `<,>,<=,>=,==,!=` are allowed
- For String data, operators such as `==,*=,!=` are allowed

For `string data`, [Geostyler](https://geostyler.org/) automatically detects all unique values so users can simply select it from a dropdown.

![string_selector]( ../images/string_selector.png "string_selector")

# AND Filter

 [Geostyler](https://geostyler.org/) allows combining multiple conditions together using boolean operators. Once  an AND filter is selected from the list, users can select further filters which again can be `and`, `or`, `comparison`, `not` .

![and_filter]( ../images/and_filter.gif "and_filter")

Data of features satisfying all conditions listed in an AND filter, are visible with the selected style.

In this example we check two conditions

1. `adm0name` == `India`
2. `pop_min` < 50000

![and_filter_in_use]( ../images/and_filter_in_use.png "and_filter_in_use")

as per condition, we get **10** features here.

# OR Filter

Using `OR` Operator, gets the results which follows any of the given conditions. Users can create combinations of `and`, `or`, `comparison`, `not` conditions as per need.

![and_or]( ../images/and_or.png "and_or")


Data of features satisfying any conditions listed in OR filter, are visible with the selected style.

In this example we check two conditions

1. `adm0name` == `India`
2. `pop_min` < 50000

![or_filter_in_use]( ../images/or_filter_in_use.png "or_filter_in_use")

as per condition, we get **3873** features here.

# NOT Filter

`NOT` filter works like an *anti-comparison* filter. As we do in `comparison` filter, we create a condition over here and all features which don’t follow that condition will be styled. 

Users can create combination of `and`, `or`, `comparison`, `not` conditions as per need.

Data of features not satisfying the condition listed in NOT filter, are visible with the selected style.

In this example we check condition

1. `adm0name` == `India`

![not_filter]( ../images/not_filter.png "not_filter")