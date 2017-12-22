---
layout: post
title: Working with APIs - Part1
category: Coding

excerpt: My personal learnings on working with APIs due React Projects.

---

# Working with APIs - Part1

### Check if an array contains a value in JavaScript
Example: we have an array containing brand names: 
`brands = ["adi, nike, puma"]`
We need to check if the array has a value or not to set the checkbox to **true** or **false**.

Our checkbox has the ID: **'nike'**;

The check itselves is easy like: `brands.includes('nike')`

#### What can go wrong:
Always check if the value in the array has the same type as your ID. (string or number or whatever.)

#### Final code:
So in my case it will look like this:
```javascript

let val = typeof value.id !== 'string' ? JSON.stringify(value.id) : value.id;

idval = brands.includes(val);
```
