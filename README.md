# REALTIME CLOCK :clock3::two_hearts:

> A Realtime clock :clock12: inspired for a project, uses `moment.js` and `jQuery`

> **Moment.js** is a javascript library for retrieving time with the help of your **IP** adress

Usage of `javascript`, `css`, `html` along with the libraries- `jQuery` & `momentjs` creates an ideal:bulb: option to choose this as a project. Use the below documentation to understand the logical making of the project. 

 ### SAMPLE CODE :o:
 ```js
 // ANALOGUE CLOCK'S TIME HANDS ADJUSTMENT MATH LOGIC
 var hrsdeg = ((hrs12 % 12) / 12) * 360 + (min / 60) * 30;
 var secdeg = (sec / 60) * 360;
 var mindeg = (min / 60) * 360 + (sec / 60) * 6;

// MOVEMENTS FOR THE CLOCK HANDS
 hrshand.css({
   transform: "rotate(" + hrsdeg + "deg)"
 });

 sechand.css({
   transform: "rotate(" + secdeg + "deg)"
 });

 minhand.css({
   transform: "rotate(" + mindeg + "deg)"
 });

 // DIGITAL CLOCK SCREEN LOGIC
  digimins.text(min)
  digisec.text(sec)
  digihrs.text(hrs12)
 ```

 Remember to initialize the js with ( jQuery 3.6.0 ):arrow_heading_down:
 ```js
 jQuery(function(){
// CODE HERE
 });
 ```

### DESIGNING THE CLOCK
Css:
```css
/*BASIC CSS FOR THE CLOCKS INIT*/
body { 
  font-size:62.5%; 
  margin:1em; 
  background:#232425;
  margin-top: 30vh; 
}

ul { 
  list-style:none; 
  margin:0; 
  padding:0 
}

#watch { 
  font-size:1em; 
  position:relative 
}
```

Here are some class-lists for the clock:

:ghost:| className | Description
|---:|:---:|:---:|
1|digital-wrap|for the digital clock numerical time values
