# Blasphemy

A simple offline javascript solution to checking and filtering profanity. Simply import [blasphemy.js](https://raw.githubusercontent.com/garrickbrazil/blasphemy/master/blasphemy.js) and get started!


The primary funciton to be used is <code>blasphemy.judge('go badword yourself, '*')</code> which will return the following response:

```javascript
{ 
   input: "go badword yourself",
   filtered: "go ******* yourself",
   isProfane: true,
   profanePhrases: ["badword"],
   error: false 
}

````

Examples and other shortcuts:
```javascript
// full service
var obj = blasphemy.judge('some input', '*');

// some other shortcuts
var string = blasphemy.censor('some input', '*');
var stringArray = blasphemy.profanePhrases('some input');
var bool = blasphemy.isProfane('some input');
```
