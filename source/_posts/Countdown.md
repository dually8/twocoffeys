---
title: Countdown
date: 2017-06-14 16:43:04
tags:
---

It's getting closer and closer to that time! Here's a countdown to help us.

{% raw %}
<h2 id="countdown">Loading...</h2>

<script>
// Set the date we're counting down to
var countDownDate = new Date("Nov 19, 2017 16:30:00").getTime();

// Update the count down every 1 second
var x = setInterval(function() {

    // Get todays date and time
    var now = new Date().getTime();

    // Find the distance between now an the count down date
    var distance = countDownDate - now;

    // Time calculations for days, hours, minutes and seconds
    var days = Math.floor(distance / (1000 * 60 * 60 * 24));
    var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((distance % (1000 * 60)) / 1000);

    // Output the result in an element with id="demo"
    document.getElementById("countdown").innerHTML = days + " days, " + hours + " hours, "
    + minutes + " minutes, and " + seconds + " seconds.";

    // If the count down is over, write some text
    if (distance < 0) {
        clearInterval(x);
        document.getElementById("countdown").innerHTML = "WE'RE MARRIED!";
    }
}, 1000);
</script>
{% endraw %}

Don't forget to [RSVP](/RSVP)!!!