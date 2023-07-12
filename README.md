# realtime-clock

 A realtime clock inspired for a project, uses `moment.js` and `jQuery`

 ## Some insights

 The clock css and html were originally the work of another developer,<br>
 I just added the jQuery to make it work in real-time.<br><br>
 My sinscere thanks for the source code.

 ### Scaling the project ?
 Well scaling this project is simple. Just use the same logic for the clock hands movement if you are going to use the analogue clock, else you can use the digital one.

 ### sample codes:
 ```javascript
 // ANALOGUE CLOCK
 var hrsdeg = ((hrs12 % 12) / 12) * 360 + (min / 60) * 30;
 var secdeg = (sec / 60) * 360;
 var mindeg = (min / 60) * 360 + (sec / 60) * 6;

 hrshand.css({
   transform: "rotate(" + hrsdeg + "deg)"
 });

 sechand.css({
   transform: "rotate(" + secdeg + "deg)"
 });

 minhand.css({
   transform: "rotate(" + mindeg + "deg)"
 });

 // DIGITAL CLOCK
  digimins.text(min)
  digisec.text(sec)
  digihrs.text(hrs12)
 ```
