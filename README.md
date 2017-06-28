# CSS Box Model
by Jonathan Ahrens

![](https://media.giphy.com/media/pkUDad439VgMU/giphy.gif)

## Class Audience  
HighSchool Students (16-18)  

## Lesson Goals
At the end of this lesson you will know
- [ ] what is the `box model`?
- [ ] the importance of `height`  
- [ ] properties that conform the box model
    - [ ] Margin
    - [ ] Border
    - [ ] Padding
    - [ ] Content
- [ ] How to set and modify these properties
- [ ] top, right, bottom, left
- [ ] Use the Google Chrome inspector


## Supposed knowledge
- [ ] how to add
- [ ] basic HTML templating
- [ ] No linking to CSS or JS (inline)
- [ ] How to target id's in CSS
- [ ] How to target classes in CSS

## Content
### HTML elements
As simple as that, ANY HTML element = BOX, that simple.  
HTML elements can be [**Inline**](https://developer.mozilla.org/en-US/docs/Web/HTML/Inline_elements) or [**Block**](https://developer.mozilla.org/en-US/docs/Web/HTML/Block-level_elements) elements. We are going to focus on the block elements.  

### Brief Introduction: Height and width 
When the box is empty, it's collapsed  
![Collapsed Box](http://www.campshippers.com/photos/box/flat.jpg)  

**Let's head over to our index.html!!**  
Let's try adding `background-color: firebrick` in the body `<body>` tag, like this:  
```css
body {
    background-color: firebrick;
}
```

Why don't we see red in the page right now? 😫 😩 😤
> If body has no content or no defined height it will not show red at all. Same goes for any block element: it's collapsed  

By adding content we can make the box appear in the HTML page...  
![Box with Cat](http://cdn2-www.cattime.com/assets/uploads/2016/08/CardboardCollapsed.png)
```css
body {
    background-color: firebrick;
    height: 100%;
}
```

### The four properties of the box-model  
![](https://www.washington.edu/accesscomputing/webd2/student/unit3/images/boxmodel.gif)  

*Margin* - most exterior space around the HTML object, it's like the force, it pushes our box away from others (INVISIBLE SPACE).  
*Border* - delimits the surroundings, like a fence. The fence **has thickness too!**  
*Padding* - the filling between our content and the border (INVISIBLE SPACE).  
*Content* - Whatever we put inside of this box (THINK KITTY ABOVE).  

We can modify the values of these by tagetting our div...  
Observe closely and let's discuss what we see...  
```css
div {
    height: 100px;
    width: 100px;
    /*with no height and width our div would not appear*/
    margin: 100px 100px 100px 100px;
    /*why four values?? ^^ any ideas?*/
    border: 20px solid black;
    /*hmmm three things, what do they mean?*/
    padding: 20px;
    /*were we not expecting 4 values here? */
}
```

**The order for these values in CSS**  
TOP, RIGHT, BOTTOM, LEFT  
`margin: 100px 100px 100px 10px`  

## Sidewalk, Fence, Garden, House example... To the whiteboard!
IMPORTANT: when you add values to each one of these they will SUM UP as part of the perimeter of the whole element (read, the bigger our values, the more garden, fence and sidewalk we are going to have). 

## Let's do some exercises
Look into `index.html` file and let's start styling:
1. Make a div, with a thick fancy border of 25px with the color `rebeccapurple`
2. Give me the dimmensions considering thickness of the box-model  

## Wrap up 
What did we learn?
- [x] box model: everything is a box in HTML
    - [x] Margin: exterior separation from the element, invisible  
    - [x] Border: delimiter of the exterior of the HTML element  
    - [x] Padding: spacing between the border and the content, invisible  
    - [x] Content: whatever you want to put there
- [x] How to set and modify these properties
- [x] top, right, bottom, left


## Resources
- [W3Schools CSS box model](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&ved=0ahUKEwi9jrbF7t7UAhVKOT4KHamxCdAQFggsMAE&url=https%3A%2F%2Fwww.w3schools.com%2Fcss%2Fcss_boxmodel.asp&usg=AFQjCNFDEcG_RtTiv54J65CJ5iyZKa4SkQ&cad=rja)  
- [Mozilla Dev Network Margin](https://developer.mozilla.org/en-US/docs/Web/CSS/margin)  
- [Mozilla Dev Network Padding](https://developer.mozilla.org/en-US/docs/Web/CSS/padding)  
- [Mozilla Dev Network Border](https://developer.mozilla.org/en-US/docs/Web/CSS/border)  


