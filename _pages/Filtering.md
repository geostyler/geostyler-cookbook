---
title: Filter
author: Krishna Lodha
date: 2022-06-07
category: functions
layout: post
---


# Filtering

Filtering allows users to create conditions based on `columns` available in the data. Depending upon `data type` of `column` (e.g. number, boolean, string, etc. ) user can select operators and use it with data available within column.

Users can also add, remove, convert one filter type into another using UI.
![change_filter]( ../images/change_filter.png "change_filter")


# Comparison Filter (Default)

Comparison filtering involves assigning column with some value and getting results out of it. 

e.g. For given data we’ll check what all `pop_min` is less than 500 

![Basic filter]( ../images/basic_filter.png "Basic filter")

Here users select `column name` next to column name [Geostyler](https://geostyler.org/) automatically adds `data type` and finally user can give input value. 

- For numeric data type, operators such as `<,>,<=,>=,==,!=` are allowed
- For String data type, operators such as `==,*=,!=` are allowed

For `string data type` [Geostyler](https://geostyler.org/) automatically detects all unique values so user can simply select it from dropdown

![string_selector]( ../images/string_selector.png "string_selector")

# AND Filter

 [Geostyler](https://geostyler.org/) allows combining multiple conditions together using boolean operators. Once AND filter is selected from list, users can then select further filters which again can be `and`, `or`, `comparison`, `not`

![and_filter]( ../images/and_filter.gif "and_filter")

Data of features satisfying all conditions listed in AND filter, are visible with the selected style.

In this example we check two conditions

1. `adm0name` == `India`
2. `pop_min` < 50000

![and_filter_in_use]( ../images/and_filter_in_use.png "and_filter_in_use")

as per condition, we get **10** features here 

# OR Filter

Using `OR` Operator, gets the results which follows any of the given conditions. users can create combination of `and`, `or`, `comparison`, `not` conditions as per need

![and_or]( ../images/and_or.png "and_or")


Data of features satisfying any conditions listed in OR filter, are visible with the selected style.

In this example we check two conditions

1. `adm0name` == `India`
2. `pop_min` < 50000

![or_filter_in_use]( ../images/or_filter_in_use.png "or_filter_in_use")

as per condition, we get **3873** features here

# NOT Filter

`NOT` filter works like an *anti-comparison* filter. As we do in `comparison` filter, we create a condition over here and all features which doesn’t follow that condition will be styled. 

 users can create combination of `and`, `or`, `comparison`, `not` conditions as per need

Data of features not satisfying condition listed in NOT filter, are visible with the selected style.

In this example we check condition

1. `adm0name` == `India`

![not_filter]( ../images/not_filter.png "not_filter")