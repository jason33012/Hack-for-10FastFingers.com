# Hack-for-10FastFingers.com
This is a hack that will automatically type in words on the website with high accuracy.
Just go to inspect then click on console and paste in this code:

var input = $('#inputfield')[0]
var ev = $.Event('keyup')
ev.which = 32
setInterval(function() {
    if ($('.highlight')[0]) {
        input.focus()
        input.value = $('.highlight').text()
        $(input).trigger(ev)
    }
}, 100)

Copy the link in raw for it to work
