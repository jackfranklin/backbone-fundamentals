## Prelude

![](img/logo.jpg)

Not so long ago, "data-rich web application" was an oxymoron. Today, these applications are everywhere and you need to know how to build them.

Traditionally, web applications left the heavy-lifting of data to servers that pushed HTML to the browser in complete page loads. The use of client-side JavaScript was limited to improving the user experience. Now this relationship has been inverted - client applications pull raw data from the server and render it into the browser when and where it is needed.

Think of the Ajax shopping cart which doesn't require a refresh on the page when adding an item to your basket. Initially, jQuery became the go-to library for this paradigm. It's nature was to make Ajax requests then update text on the page and so on. However, this pattern with jQuery revealed that we have implicit model data on the client side. With the server no longer being the only place that knows about our item count, it was a hint that there was a natural tension and pull of this evolution. 

The rise of arbitrary code on the client-side which can talk to the server however it sees fit has meant an increase in client-side complexity. Good architecture on the client has gone from an afterthought to essential - you can't just hack together some jQuery code and expect it to scale as your application grows. Most likely, you would end up with a nightmarish tangle of UI callbacks entwined with business logic, destined to be discarded by the poor soul who inherits your code.

Thankfully, there are a growing number of JavaScript libraries that can help improve the structure and maintainability of your code, making it easier to build ambitious interfaces without a great deal of effort. [Backbone.js](http://documentcloud.github.com/backbone/) has quickly become one of the most popular open-source solutions to these issues and in this book we will take you through an in-depth walkthrough of it.

Begin with the fundamentals, work your way through the exercises, and learn how to build an application that is both cleanly organized and maintainable. If you are a developer looking to write code that can be more easily read, structured, and extended - this guide can help.

This book is released under a Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported [license](http://creativecommons.org/licenses/by-nc-sa/3.0/) meaning you can both grab a copy of the book for free or help to further [improve](https://github.com/addyosmani/backbone-fundamentals/) it. Corrections to existing material are always welcome and I hope that together we can provide the community with an up-to-date resource that is of help.

My extended thanks go out to [Jeremy Ashkenas](https://github.com/jashkenas) and [DocumentCloud](documentcloud.org) for creating Backbone.js and [these](https://github.com/addyosmani/backbone-fundamentals/contributors) members of the community for their assistance making this project far better than I could have imagined.

## Target Audience

This book is targeted at novice to intermediate developers wishing to learn how to better structure their client-side code. An understanding of JavaScript fundamentals is required to get the most out of it, however we have tried to provide a basic description of these concepts where possible.

## Acknowledgements

I am indebted to the fantastic work done by the technical reviewers who helped improve this book. Their knowledge, energy, and passion have helped shape it into a better learning resource and they continue to serve as a source of inspiration. Thanks go out to:

* [Marc Friedman](http://github.com/dcmaf)
* [Derick Bailey](https://github.com/derickbailey)
* [Jeremy Ashkenas](https://github.com/jashkenas)
* [Samuel Clay](https://github.com/samuelclay)
* [Mat Scales](http://github.com/wibblymat)
* [Alex Graul](https://github.com/alexgraul)
* [Dusan Gledovic](http://github.com/g6scheme)
* [Sindre Sorhus](http://github.com/sindresorhus)

## Credits

None of this would have been possible without the time and effort invested by the other developers and authors in the community who contributed to it. I would like to extend my thanks to Derick Bailey, Ryan Eastridge, Jack Franklin, Mike Ball, Uģis Ozols, Björn Ekengren and our other excellent [contributors](https://github.com/addyosmani/backbone-fundamentals/graphs/contributors) that made this project possible.

## Reading

I assume your level of knowledge about JavaScript goes beyond the basics and as such certain topics such as object literals are skipped. If you need to learn more about the language, I am happy to suggest:

* [JavaScript: The Definitive Guide](http://shop.oreilly.com/product/9780596805531.do) by David Flanagan (O’Reilly)
* [Effective JavaScript](http://www.informit.com/store/effective-javascript-68-specific-ways-to-harness-the-9780321812186) by David Herman (Pearson)
* [JavaScript: The Good Parts](http://shop.oreilly.com/product/9780596517748.do) by Douglas Crockford (O’Reilly)
* [Object-Oriented JavaScript](http://www.amazon.com/Object-Oriented-Javascript-Stoyan-Stefanov/dp/1847194141) by Stoyan Stefanov (Packt Publishing)

