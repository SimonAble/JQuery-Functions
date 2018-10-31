## JQuery Functions

This repository contains a bunch of implementations for common JQuery functions. This can serve as a nice reference for those looking to understand the basic methods for creating different visual effects in JQuery.

You can play around with a bunch of these functions by clicking <a href = "https://simonable.github.io/JQuery-Functions/">Here</a>

![](https://github.com/SimonAble/JQuery-Functions/blob/master/img/Screen%20Shot%202018-10-30%20at%208.42.02%20PM.png)

### Functions covered in this repository:

- .click
```javascript
//Click Button
$("#click_bttn").click(function(){
  $("#click").fadeToggle("Button Clicked!");
  $("#pclick").html("Hey, you clicked the button! Click it again to see what happens.");
})
```

- .hide
```javascript
//Hide Button
$("#hide_bttn").click(function(){
  $("#hide").hide();
  $("#phide").html("Ah! That looks much better.")
});
```

- .show
```javascript
//Show Button
$("#show_bttn").click(function(){
  $("#hide").show();
  $("#pshow").html("I think it looks better that way, don't you?")
  $("#phide").html("Thanks for putting me back!")
});
```

- .fadeToggle
```javascript
//Toggle
$("#toggle_bttn").click(function(){
  $("#hide_func").fadeToggle();
  $("#show_func").fadeToggle();
  $("#ptoggle").html("Muahahaha. It must be WITCHCRAFT! You can always bring it back by clicking the button again...at least, I hope.");
});
```

- .slideUp
```javascript
//Slide Up
$("#slideUp_bttn").click(function(){
  if ( $( "#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func" ).is( ":hidden" ) ) {
      $( "#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func" ).slideDown( "slow" );
  } else {
      $( "#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func").slideUp("slow");
  }
  $("pslide").html("Slide to the left... slide to the right!")
});
```
- .slideDown
```javascript
//Slide Down
$("#slideDown_bttn").click(function(){
  if ( $( "#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func" ).is( ":hidden" ) ) {
      $( "#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func" ).slideDown( "slow" );
  } else {
      $( "#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func").slideUp("slow");
  }
});
```

- .slideToggle
```javascript
//Slide Toggle
$("#slideToggle_bttn").click(function(){
  $("#click_func,#hide_func,#show_func,#toggle_func,#slideUp_func,#slideDown_func").slideToggle("slow", function(){

  });
}); 
```

- .fadeIn
```javascript
//FadeIn
$("#box-contain").hide();

$( "#fadeIn_bttn" ).click(function() {
    $( "#box-contain" ).fadeIn( "slow", function() {
// Animation complete
    });
});
```

- .fadeOut
```javascript
//FadeOut
$( "#fadeOut_bttn" ).click(function() {
    $( "#box-contain2" ).fadeOut( "slow", function() {
// Animation complete
    });
});
```

- .addClass
```javascript
//Add Class
$("#addClass_bttn").click(function(){
  $("#addClass_bttn").addClass("button2");
  $("#addClass_func").addClass("func_contain2");

})
```

- .before
```javascript
//before
$("#before_bttn").click(function(){
  $( "#pbefore" ).before( "<b>Perfect! Thanks for putting me before all else :P</b>" );
})
```

- .after
```javascript
//after
$("#after_bttn").click(function(){
  $( "#pafter" ).after( "<b>It looks like I'm not that important after all!</b>" );
})
```

- .append
```javascript
//append
$("#append_bttn").click(function(){
  $("#img_cont").append('<img src="img/ninja.jpg"/>');
  $("#pappend").html("Someone is hiding below. I wonder what it could be. Scroll down if you dare!")
})
```

- .html
```javascript
//html
$("#html_bttn").click(function(){
  $("#phtml").html("Out with the old, in with the new!");
})
```

- .attr
```javascript
//attr
$("#attr_bttn").click(function(){
  $( "#galaxy_img" ).attr({width: "100%", height:"100%"});
})
```

- .val
```javascript
//Value
$("#val_bttn").click(function(){
  $("input:text").val("I have value now. THANK YOU!");
})
```

- .text
```javascript
//Text
$("#text_bttn").click(function(){
  $("#ptext").text(function(){
  return "Like this, this is incredible content!";
  });
})
```

