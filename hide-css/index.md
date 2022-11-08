---
title: Using JavaScript to Hide CSS
layout: content
---

## Using JavaScript to Hide CSS

Suppose you want to hide elements of a page -- e.g., every event in an EveryAction events calendar with the word Public in its title. Here's what you need to do:

1. Use the
to find out what CSS tag
[CSS tag]( https://developer.chrome.com/docs/devtools/css/)

2.

[Example](hide-private-events.html)

https://www.w3schools.com/howto/howto_js_add_class.asp

Basically, the strategy most folks use is create a class that has the CSS in it you that you want to use—e.g., CSS that makes the element not display -- and then have a little JavaScript attached to a button or whatever that adds the class to the element/elements we want to hide.

And here's the CSS to make something not visible:
https://www.w3schools.com/cssref/pr_class_visibility.asp

And if that doesn't work, we may need to add something to our CSS that says, this one is the priority, a.k.a. !Important:
https://www.w3schools.com/css/css_important.asp




What I learned:

 You can use a class to hide an element:
        .private-event {
            visibility: hidden;
            padding: 0px;
        }
        // event.classList.add("private-event");

The problem you may run into is that if there is padding, etc., getting it to work is a real pain

So, you are better off removing the entire element