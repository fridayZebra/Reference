# Reference material while learning Javascript
- [ ] get this better organized!

=============================
### Javascript
  
[Array Practice Drills](https://www.w3resource.com/javascript-exercises/javascript-array-exercises.php)


1. Books

    [You Don't Know JS Series](https://github.com/getify/You-Dont-Know-JS/blob/master/README.md)  
    [Exploring ES6](http://exploringjs.com/es6/index.html#toc_ch_about-book)  
    [Learning JavaScript Design Patterns v1.7.0](https://addyosmani.com/resources/essentialjsdesignpatterns/book/)  
    [Eloquent Javascript 2nd Ed](http://eloquentjavascript.net/index.html)  

2. Fundamentals  
    [Javascript Basics](https://autotelicum.github.io/Smooth-CoffeeScript/literate/js-intro.html#arrays)  
    [jQuery Fundamentals](http://jqfundamentals.com/chapter/events)  
        - Events and Event Delegation

2. OOP  
    [JS Objects in Detail](http://javascriptissexy.com/javascript-objects-in-detail/) [Very Thorough]  
    [Object Playground](http://www.objectplayground.com)  
        - good explanation on prototype and inheritance in 30 min video

3. Misc JS  
    [Build 30 Things in 30 Days](https://javascript30.com) [Do this when time alows]  
    
=============================  

### HTML
[Dive into HTML5](http://diveintohtml5.info)

[MDN Reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)

[Good Class Names W3](https://www.w3.org/QA/Tips/goodclassnames)  

=============================
### CSS
[Flexbox Froggy](http://flexboxfroggy.com)

[Learn CSS Layout](http://learnlayout.com/toc.html)

[7 Principles of Clean/Optimized CSS](https://www.smashingmagazine.com/2008/08/7-principles-of-clean-and-optimized-css-code/)

[Getting to Know CSS](https://learn.shayhowe.com/html-css/getting-to-know-css/)

[Responsive Patterns](https://bradfrost.github.io/this-is-responsive/patterns.html)

#### CSS Tricks
[Centering in CSS: A Complete Guide](https://css-tricks.com/centering-css-complete-guide/)

[Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

=============================
#### 1. Node/NPM  
   ##### a. Shortcuts  
   *long form*  
   + npm install --body-parser  
  **shorthand**  
    + npm i -S body-parser

##### b. Dev Dependancies (installed just on dev local machine)  
  **long form**  
     - npm install --save-dev morgan  
  **shorthand**
     - npm i -D morgan

   #### 2. Misc/Good to Know  
   - .gitignore => in file at tope, write node_modules (this keeps node from being pushed to repo)  
   - Heroku only runs dependancies, not devdependancies  

=============================
   

### Redux 'Tricks'  
- use this to be able to see previous and next state in the console

```javascript
//will likely need to install redux-logger
//npm i --save redux-logger

import { createStore, compose, applyMiddleware } from "redux";  //add compose and applyMiddleware for prev/action/next state
import {createLogger} from 'redux-logger';  //for prev/action/next state
import { connect } from "react-redux";

import { reducer } from "./reducers";

export default createStore(reducer,
  undefined, //for prev/action/next state
  compose(    //for prev/action/next state
    applyMiddleware(createLogger()),  //for prev/action/next state
    window.devToolsExtension ? window.devToolsExtension() : f => f  //for prev/action/next state

  )
);


//the additions and changes to 
//line 4, 5, 11-16
//are all needed to make the prev/action/next state show up in the console
```

---
### Formatting Markdown

- [GitHub Guides](https://guides.github.com/features/mastering-markdown/)

- [Markdown Cheat Sheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

=============================
### Linux Mint 18.3 Cinnamon Install on Win 10 
12/3/17  
if install stalls, use nomodeset  
   - seems to be needed with specific video cards, in my case: nvidia  
   - found info at linux form site  
   - mint website directs you to do this, but the step where they say to choose the nvidia driver may be incorrect. follow instructions [here:](https://forums.linuxmint.com/viewtopic.php?t=122257)  
   - tells you how to use the xforcevesa driver so when you start up, the nvidia driver isn't in use and can actually be applied

[Installing Chrome](https://winaero.com/blog/install-google-chrome-linux-mint-18/)  

=============================  
### Misc Web How/What/Why
[obs-studio](https://github.com/jp9000/obs-studio/wiki/Install-Instructions#debian-based-build-directions)  
- overlay that lets you share windows, not screens  
[obs-websocket](https://github.com/Palakis/obs-websocket)  
[obs-linuxbrowser](https://github.com/bazukas/obs-linuxbrowser) 

jquery reminder  
[jquery](https://www.youtube.com/watch?v=Pt49y1gm0jw&list=PLqGj3iMvMa4KOekRWjjajinzlRK879Ksn)
