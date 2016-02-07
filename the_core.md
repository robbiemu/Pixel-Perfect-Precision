# The Core

_"This ﬁrst section covers core principles and topics that apply to digital design and its relevant tools. Applicable to both seasoned professionals and newcomers to the ﬁeld, it offers a quick start guide to some of the processes and thinking that we apply to our projects here at ustwo."_

## Users

Right away they start with a rather strange example:

    a completely ﬂat, cutting edge interface guided by grids and typography may work for a younger audience, but perhaps some friendlier skeuomorphic touches would be more appropriate for older users who aren’t quite so tech-savvy.

### Skeuomorphic

I had to look it up. It is something with illustrative flurishes that decorate. Here is a concrete example, next to flat design:

![](https://www.pulldigital.com/getmedia/8d04e286-dac3-4c52-bbd1-5677319ff575/calendar.jpg)

The thing is, no one wants the seuomorphic design in this example. So it isn't a good one.

Similarly with a practical example:

![](http://www.eightytwenty.ie/blog/wp-content/uploads/2013/09/skeuomorphic-11.jpg)
![](https://axc3670.files.wordpress.com/2014/05/calculator.png)

We face the same problem. The older design, while reflective of a history, doesn't better inform us or provide any signficant advantage. In fact it just looks rather hokey.

Better are these examples, where clearly preference can be personal:

![](http://www.jacksonwynne.com/2015/wp-content/uploads/2013/02/skeumorphism-iphone-lumia-flat-design.jpg)
![](http://www.forward.ph/blog/wp-content/uploads/2013/07/Skeuomorphism-or-Flat-Design-Forward-Solutions.png)

## Environment

I find it interesting to consider this page relative to responsive design. In responsive design you try to repurpose the same page data to different layouts based on the relative pixel of the web browser — since smaller screens use _virtualized pixels_ to give you legible text on smaller pages, you end up with less pixels on thes viewports. The designer can then specify css styles like

    @media (max-width: 640px) { 
        @viewport{ width: 640px; } 
        html { font-size: 10pt; /* ...style.. */ }
        /* etc */ 
    }

In this way the page can respond to the device. But they point out there are also considerations about the environment the device is purposed for. A mobile device has to stand up to sunlight, for example. A flat, ie plain, unadorned (non-skeuomorphic) design makes sense when screen size and lighting conditions compete with any detail in the visual content. Similarly you'd probably want sounds to be clear, simple, and even more sparing in use than on the desktop. This doesn't necessarily change things for designers, but the next one might: Your color palette could stand to be a bit more contrasty and saturated on devices that might be used outdoors.

## Accessibility

They provide a nice write up showing that _less is more_, and the text highlights clarity as a design goal in cmmon with accessibility.

## Worst-case Scenarios

In this section they illustrate the need to ensure that dynamic data will look good in the design. The goal is to consider the details being shown, to ensure that clipping doesn't have to occur.

See this [jsFiddle](https://fiddle.jshell.net/w07ww20q/1/) illustrating both concerns (source files are available under the worst-case-scenarios folder, in case the jsfiddle url is deregistered later).

#