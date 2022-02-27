# Space Tourism Webpage

#### Frontend Mentor challenge

![Design of the Homepage at 1920x1080p resolution](./Screenshot1.png "Design of the Homepage on 1080p screen")

## Welcome

This site uses purely `.html` and `.css` to achieve all its design challenges. But because of that, the site has certain quirks that I want to disucss.

But first lets go through what I was able to achieve through this challenge.

## Overview of some the things I learnt along the way

+ Some solid Google-fu to find out the ways internet solve their problems similar to mine. Many consider this to be a key skill and while searching a solution might not be difficult, it's the implementation of their said solution into our project that matters.
+ Pre-planning the layout of HTML to make life easier while writing the CSS stylesheet.
+ The uses, precedence and priority of HTML tags, class and id and other combination of selector to select specific element without too much clutter and confusion.
+ The importance of `meta` tag to specfically tell screens to scale according to phone screens.
+ Use of `div` to wrap around elements and control them effectively.
+ Using flexbox as an powerful way to arrange (and rearrange) the different elements of HTML and also most convenient way to center elements.
+ Checkboxes of CSS as condtional to implement very basic level of dynamic behavior.
+ **A nice filter/frost effect that works on all browsers because Firefox at the moment doesn't support `backdrop-filter`.** This one took a lot of headbanging 😂. CSS Pseudo-class are a way to implement interesting design techniques.
+ The sidebar implementation on the mobile version of the page is probably a big learning point for me. And it also showed me while a javascript appraoch might make it a lot more simpler / easier to understand.

## Achievements

Users should be able to:

+ View the optimal layout for each of the website's pages depending on their device's screen size
+ See hover states for all interactive elements on the page
+ View each page and be able to toggle between the tabs to see new information

## Quirks

- No caraousel implementation that most users will probably expect [on this page](https://arkni8.github.io/space-tourism-webpage/html/crew-pilot.html)
- The frost effect of navigation/sidebar looks mostly great but if you look too closely, you will find unblurred image at the edges of the screen. This is a limitation of the `filter: blur()` and I have yet to find a workaround for it.
- It doesn't support hot reload, so every link reloads the page, but since the pages itself are small, I didn't think it matters too much.
- Debbugging the CSS might be tough since the codes are lengthy and while I have tried my best to refactor the code, its still lengthy. I have divided the CSS into two parts, one part dealing with just the navigation header, and the other part dealing with just styling the rest of the body.
- The media queries make the responsive logic especially lengthy. Is there a way to make a more responsive page without writing that media queries like I have? I don't have an answer to that yet.

### Some points to discuss

+ Initially I added Bootstrap to help with building responsive layouts faster. But I found out very soon that when you have a lot of custom elements and design, controlling Bootstrap becomes a lot more challenging as you try to contest the CSS of Bootstrap elements. That is when I also learned that stylesheet precedence also matters when you insert it at the header of a HTML. **So always insert Bootstrap stylesheet over all the custom stylesheet, and not doing so is going to cause a lot of headache.** The scripts are also prewritten and modifying them is a lot more painful, so in the end, its just better to design the page ground up. It was definitely a lot faster than fumbling with default behavior of Bootstrap.
+ Using CSS Pseudo-class was a genius move made by gentlemen on StackOverflow. Some were able to use Pseudo-class trick CSS into adding effect that I was not able to otherwise. I improvised his idea and implemented it in another form on this website. [Here is a demo.](https://codepen.io/betravis/pen/xxGPJm)
+ After removing Bootstrap, I had to rely on pure CSS to implement Sidebar and I just followed [this very simple idea](https://codepen.io/plavookac/pen/qomrMw) to make the sidebar work. After that, it was just a couple of media queries away from having a  fully responsive site.
  
