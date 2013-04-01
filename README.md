JQueryLinedText
===============

One of the most used, but under featured HTML controls, is the humble TEXTAREA control. This control is designed to accept large blocks of text from the user. A wide variety of plugins exist for the TEXTAREA that layer it with toolbars, auto-resizing, rich-text editing and the works.

However, for my usage, this was way over kill. I wanted a simple line-number facility that would allow my users easily see where they are. Particuraly handy for editing code online. After searching, I couldn't find one, so I simply created my own plugin.


Quickly and easily to install, very light weight, you simply tell it which TEXTAREA's you want to be line tracked and it will go and do its thing. You can pass if you want a line highlighted. While it doesn't highlight the line inside the TEXTAREA control it highlights the side bar at the relevant place.

<pre><script>
$(function() {

  // Target all classed with ".lined"
  $(".lined").linedtextarea(
    {selectedLine: 1}
  );

  // Target a single one
  $("#mytextarea").linedtextarea();

});
</script>
</pre>

Installation: Copy the files to your web server and insert the .js and .css file and you are good to go. Requires JQuery 1.3+
