# Media Queries

### @media

CSS uses the @media rule to detect information about the device being used to access the website. 

We have three basic categories of devices: phones, tablets, and desktops. We will focus on using media queries to detect which category of device is being used and respond appropriately. 

| Device        | Size                                  |
| ------------- |:-------------------------------------:|
| Phone         | Width less than or equal to 480px     |
| Tablet        | Width between 481px and 1023px        |
| Desktop       | Width greater than or equal to 1024px |


### Example

Let's say that we have four buttons on our website that we would like to change color depending on the size of the screen. We'll give desktop users red buttons, tablet users blue buttons, and phone users yellow buttons. We'll give the buttons the class of ```.navbtn```.

To get you started, here's how we would set up a media query in our CSS to notice if the user's screen is 480 px wide or smaller. If this is true, then we will target all elements with the class ```.navbtn``` and set their background to be yellow.

```
@media only screen and (max-width: 480px){
     /* we will set these stylings only if the device is a screen with a width of 480px or less */
     .navbtn {
         background-color: yellow;
     }
}
```


Remember that CSS is read from top to bottom, so if the conditions of the media query are met, the stylings within could override any stylings you placed on .navbtn in the code above the media query. Any code that you write below the media query may override the stylings we did here.

Try changing the button colors from red to blue to yellow on your own, depending on screen size. Rewatch the video above if you need a hint. Then, change how the buttons are oriented depending on screen size.

* For desktop users, arrange all four buttons in one line
* For tablet users, place two buttons per line
* For phone users, give each button its own line


