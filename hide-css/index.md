---
title: Using JavaScript to Hide CSS
layout: content
---

## Using JavaScript to Hide CSS

Suppose you want to hide elements of a page -- e.g., every event in an EveryAction events calendar with the word Public in its title. Here's what you need to do:

1. Use Google Chrome's Developer Tools to find out what the [CSS tag]( https://developer.chrome.com/docs/devtools/css/) is the element you want to manipulate.

2. Add some JavaScript that loops through each element containing that tag, and if the element has the word/words you are searching for, remove that element.

Here's a simple example:
- The [sample code](https://github.com/aschneiderman/javascript-samples/blob/main/hide-css/hide-private-events.html)
- The [code in action](hide-private-events.html)


In theory, another way to go would be to add a CSS class that hides the event. For example:
```
        .private-event {
            visibility: hidden;
            padding: 0px;
        }
```

And then add a line of JavaScript that looks something like this:
```JavaScript    
event.classList.add("private-event");
```

The problem you may run into is that if there is padding, etc., getting it to work is a real pain

So, you are better off removing the entire element.
