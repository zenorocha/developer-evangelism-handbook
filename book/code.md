## Write excellent code examples

Code examples are what makes your posts and articles very relevant to developers. They say more than dozens of pages about a certain product and – even more importantly – they invite people to play with your products.

## Solve a problem with your example

One of my biggest bug-bears are “hello world” examples that don't do anything useful. Instead I aim to give out code that solves a real problem. I will come back to the “hello world” dilemma in the [presentation tips chapter](tips.html#avoid"helloworld") but for now, let's just say that writing **“hello world” code teaches people to write code, but not how to solve issues with it**.

Good code examples should answer the “how does this technology help me solve a problem?” and not the “how do I use this?” question. The“how do I use this?” question can be answered by documentation. Code examples should get people excited about using the product and entice them to dive into the documentation to find out about the details.

So instead of starting by reading the docs yourself, check what the tool can do and look for a problem you always wanted to solve that can be solved with this technology. Then solve it using the product and explain what you've done as the code example.

## Show a working example

One of the first things to show in a code example is a working implementation. There is nothing more powerful than a way to see what the thing does by clicking a link or entering some data and sending off a form. You telling the readers that it works is one thing – the readers being able to try it out and seeing it for themselves is much more rewarding.

> **Tip:** If the code you explain is part of a larger interface, behind a firewall or needs authentication then you can still show how it works by recording a screencast.

The working examples should of course work but also be pretty and smooth. A lot of examples fail to please the eye or actually violate a lot of usability basics – don't give a shoddy first impression.

## Explain the necessary environment

One of the things you want to avoid is people getting excited about your code and then not being able to make it work in their own environment. You get around this issue in several ways:

* **Write defensive code** – check for dependencies before trying to access them.
* **Check online and HTTP status** – If your code needs to pull data from a web service say that the user needs to be online to run it. For example I've had many a complaint that my Ajax examples don't work offline or without running a localhost. Obviously I failed to explain that Ajax is meant to work over HTTP.
* **List what is needed** – say what your specs are, f.e. “needs PHP5 with cURL and imageMagick” or “Firefox 3.5, Opera 9 or Safari 4 needed”.
* **Provide a simple test script** that checks for the right setup. (For an example see the [test file for GeoMaker](http://github.com/codepo8/GeoMaker/blob/3d88e693698965b802539d2a467e05f1f67cff76/test.php)).
* **Provide a developer key for the demo** – but make it obvious to tell people that to implement your code they'd need an own key. Provide a link where to apply for one.

You won't be able to predict all things people can do wrong when implementing your code but these are some good ways of preventing frustration. Which brings me to a very important part of code examples: allowing for copy and paste.

## Write working copy and paste code

Copy and paste is probably the most used way of learning code. You can write documentation until your fingers bleed, but the biggest use case is that developers will check a code example, copy and paste it, fiddle around with it until they get stuck and then start reading the docs.

Therefore it is immensely important to **write very good copy and paste examples**. Any bad coding habit you add in your code will be copied and become part of a live implementation.

Copy and paste examples that don't work are not only useless but also disastrous to your reputation and very frustrating for implementers. Therefore make sure that the following points are covered:

* **Link all resources** – point images, CSS and script resources to web locations rather than linking them locally or relative. People will copy the code and paste it in a local HTML file and not download the dependencies.
* **Provide the full script upfront** – people will copy and paste chunks of a script and complain that they don't work without realising that other parts are missing.
* **Validate and secure your code** – copy and paste code needs to be excellent as in many cases it will be what people use. Make sure your code plays well with other code and doesn't cause any warnings or errors.

> **Tip:** The best way to keep code examples and code in sync is to generate the code from the source comments. I've written a PHP script that does that for me called Tutorialbuilder which automatically applies some of the tips here.

## Have the example as a download

Providing the demo code for download as a zip file should be one of the first things you do in your example. You can ask readers to download, unpack it and code along with you (this works well with screencasts and video tutorials).

In any case it keeps your article in the mind of the readers as they have something on their hard drives reminding them of it.

Offering a zipped version of your demo code can be annoying as every change means you have to re-pack the demos. Luckily by using a hosted code solution like [GitHub](https://github.com) this job is done for you automatically.

## Write clean and clever examples

Again, I cannot stress enough that **your code examples should be the cleanest and cleverest code you ever write**.

It is very tempting to show a quick and dirty solution to get people going and earn immediate kudos for creating the shortest code ever but this is what coders do to impress each other and not what evangelists do.

You want to **show how to write excellent solutions** with the product you evangelize and every shortcut you take will be copied and taken as an excuse not to write excellent code in live projects. This is not what we are here for.

On the contrary – demo code can advertise best development practices and show them in context rather than just as an academic exercise. Showing a JavaScript that protects scope by using the Module pattern and uses closures cleverly allows you to cross-link to these ideas and maybe get some developers to take them on as part of their coding habits.

## Build code generators

A very nice touch to add to a solution are code generators that allow implementers to just add some parameters, hit a button and get the code they wanted. This is amazingly powerful.

> **Example:** Probably the most impressive example of this is Dav Glass' [Grids Builder](http://developer.yahoo.com/yui/grids/builder/) which made it dead easy for people to use the [YUI grids](http://developer.yahoo.com/yui/grids/) without needing to learn all the class names and IDs. Another success I had lately was [GeoMaker](http://icant.co.uk/geomaker) showing off the power of [Placemaker](http://developer.yahoo.com/geo/placemaker).

The only danger there is that some people will never bother learning the real implementation tricks, but on the other hand these readers are not likely to do that anyways. In any case you'll get a lot more people look at the product.
