# The Core

_"This ﬁrst section covers core principles and topics that apply to digital design and its relevant tools. Applicable to both seasoned professionals and newcomers to the ﬁeld, it offers a quick start guide to some of the processes and thinking that we apply to our projects here at ustwo."_

## Users

Right away they start with a rather strange example:

> a completely ﬂat, cutting edge interface guided by grids and typography may work for a younger audience, but perhaps some friendlier skeuomorphic touches would be more appropriate for older users who aren’t quite so tech-savvy.

### Skeuomorphic

I had to look it up. It is something with illustrative flurishes that decorate. Here is a concrete example, next to flat design:

![](https://www.pulldigital.com/getmedia/8d04e286-dac3-4c52-bbd1-5677319ff575/calendar.jpg)

The thing is, no one wants the skeuomorphic design in this example. So it isn't a good one.

Similarly with a practical example:

![](http://www.eightytwenty.ie/blog/wp-content/uploads/2013/09/skeuomorphic-11.jpg)
![](https://axc3670.files.wordpress.com/2014/05/calculator.png)

We face the same problem. The older design, while reflective of a history, doesn't better inform us or provide any signficant advantage. In fact it just looks rather hokey.

Better are these examples, where clearly preference can be personal or informative:

![](http://www.jacksonwynne.com/2015/wp-content/uploads/2013/02/skeumorphism-iphone-lumia-flat-design.jpg)
![](http://www.forward.ph/blog/wp-content/uploads/2013/07/Skeuomorphism-or-Flat-Design-Forward-Solutions.png)

## Environment

I find it interesting to consider this core design principle relative to responsive design. In responsive design you try to repurpose the same page data to different layouts based on the _device pixel_ of the web browser — since smaller screens use virtualized pixels to give you legible text on smaller pages, you end up with less pixels on these viewports. The designer can then specify css styles like

    @media (max-width: 640px) { 
        @viewport{ width: 640px; } 
        html { font-size: 10pt; /* ...style.. */ }
        /* etc */ 
    }

In this way the page can respond to the device. But they point out there are also considerations about the environment the device is purposed for. A mobile device has to stand up to sunlight, for example. A flat, ie plain, unadorned (non-skeuomorphic) design makes sense when screen size and lighting conditions compete with any detail in the visual content. Similarly you'd probably want sounds to be clear, simple, and even more sparing in use than on the desktop. This doesn't necessarily change things for designers, but the next one might: Your color palette could stand to be a bit more contrasty and saturated on devices that might be used outdoors.

## Accessibility

They provide a nice write up showing that _less is more_, and the text highlights clarity as a design goal in common with accessibility.

## Worst-case Scenarios

In this section they illustrate the need to ensure that dynamic data will look good in the design. The goal is to consider the details being shown, to ensure that clipping doesn't have to occur.

See this [jsFiddle](https://fiddle.jshell.net/w07ww20q/1/) illustrating both concerns (source files are available under the worst-case-scenarios folder, in case the jsfiddle url is deregistered later).

## Affordance

> Affordance is an object’s ability to convey its function through sensory means, for example a button suggests that you press it by being slightly raised ...

An example of _bad affordance_ you might run into in real world site design are text areas that have no borders. Another, maybe more common example, are details pages that are specified as completely separate pages that require a GET request: leaving the user feeling like they have visited a remote island in your information chain, and tempting them to use the back button.

## Copy

The approrpiate voice and coverageh for the text is important. Overly formal text can seem uninviting in more familiar contexts. Completely casual copy can seem unprepared in more formal contexts. In general, regardless of the context, the text must be informative and motived (that is, motiviating the reader).

## Color and Shape

Color and shape should agree with intent. Using a graphic "x" mark on a checkbox form input would contradict uses where it is _opt-in_, but perhaps remain appropriate for _completed_ uses. Using a red checkmark would be bad, because red suggests stop instead of go.

## Visual Hierarchy

The color, font, and layout should emphasize the parts of the page you want the user to look at,with the most important clearly standing out the most. The example on this page is one of the best examples in the early part of the book.

## Typography

I know something about this, having worked at a font company for more than 2 years. They do what most coverage does, which is to give some general info without really being specific — but this is okay because this section just touches on core principles. If I were to write up a cheat sheet for typography, it would include:

* Title should be up to 3 times the size of the text, for textual material. For graphic material, scale can vary.
* Thin, but not very thin text is okay for body.
* Serif, display, etc fonts are best for title and dropquotes. Sans-serif is best for body.
* The space between lines should normaly be the same size as the visual height of the copy. The reverse is true for graphic font use: the shorter the line height you can get away with, the more power it will carry.
* People are uncomfortable reading long lines. You often hear guidance like 60em width for body, 30em or less for columns. In general, for the line length, _less is more_.

## Motion

I'm not sure this even _belongs_ as a core idea, myself.

Motion is something they don't cover very well, at least here at the overview of core ideas. A scary exerpt is the final thought on the topic:

>  for example, if you wanted to draw attention to a new button you could make it periodically bounce to catch a user’s eye.

This is true, and it highlights what you can do with animations. It doesn't highlight _why_, or _what to avoid_. You want animation queues to be **short-lived**, **subtle**, and not hurry or distract the user.

## Testing & Prototyping

Moving from UX mock-up to the prototype of an actual design, before running live with it, is important. They make a point that, for dynamic projects, you want to actually work with live sample data before going to production with a product.

## Organization

The same project organization you might be familiar with as a programmer occurs with image, ad, and page production. They illustrate a basic project like:

* Design
...* psd files
* Assets

etc. In my own work, I often group source material together in the root folder unless it gets to be rather big.

> Good organisation is essential as it saves a lot of time for other people on the project; well ordered ﬁles and layers mean other designers can jump straight into your work and ﬁnd their way around
