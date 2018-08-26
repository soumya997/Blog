+++
date = "2018"
title = "Get In Touch"
+++

<form action="/thankyou" method="post" name="Contact" data-netlify="true" netlify-honeypot="bot-field" netlify>
    <p style="visibility: hidden">
        <label> Don't Fill This Out If You're Human:" </label><input name=bot-field/>
    </p>
    <label for="fname">First Name</label>
    <br>
    <input type="text" id="fname" name="firstname" placeholder="Your first name..">
    <br>
    <br>
    <label for="lname">Last Name</label>
    <br>
    <input type="text" id="lname" name="lastname" placeholder="Your last name..">
    <br>
    <br>
    <label for="email">Email</label>
    <br>
    <input type="text" id="email" name="email" placeholder="email@example.com">
    <br>
    <br>
    <label for="message">Message</label>
    <br>
    <textarea id="message" name="message" placeholder="Write Something Interesting" style="height: 200px"></textarea>
    <br>
    <br>
    <div data-netlify-recaptcha></div>
    <br>
    <br>
    <input type="submit" value="Submit" style="">
</form>