# css variables, favicons, @import



## css variables

[NewForce CSS Variable chapter](https://github.com/NewForce-at-Mountwest/client-side-mastery/blob/master/book-3-the-initiate/chapters/CSS_VARIABLES.md "NewForce")

### CSS Variables are sometimes referred to as Custom Properties </h1>
    CSS variables are entities defined by CSS authors that contain specific values to be reused throughout a
        document.


### Syntax to declare a variable:
+ begin with -- (maybe a nod to BEM)
+ is case sensitive
+ (e.g., --main-backgroundcolor: #1F2833;)
+ (e.g., --main-textColor: #66FCF1;)
+ add inform for common naming conventions

 ### Syntax to use a variables
 + property: var(--name);</li>
 + example => background-color: var(--main-backgroundcolor)
 + another example => color: var(--main-textColor);
 
 
````
main.css
        
:root {
    --main-backgroundColor: #1F2833;
    --main-textColor: #66FCF1;
}

h1 {
    background-color: var(--main-backgroundColor);
    color: var(--main-textColor, white);
}

````
The sample code added the variables to the :root pseudo-class, which makes its value available globally and can be used for anything inside the <html> element. 

## Add a favicon, tab icon, URL, etc to a webpage or bookmark

favicons are "square" images such as 16×16, 32×32, 48×48, 64×64, etc. pixel sizes after all [it's hip to be a square](https://www.youtube.com/watch?v=KqAamXcD_nQ). 

You can add the following line of code to your head section of an html to add the NewForce icon as a favicon.

````
<link rel="shortcut icon" href="https://raw.githubusercontent.com/kimpreece/cssVariables/master/NF.ico" type="image/x-icon">
````
There are many tools online that you can use to create .ico file types such as https://www.favicon-generator.org/

Other image file types can be used as well for favicons such as .png, .jpg and .gif; just remember to change the MIME type in the code.  For example if you are using a gif format, the code would be `type="image/gif"` instead of `type="image/x-icon"`. 

## Links to color palettes
https://visme.co/blog/website-color-schemes/. 

https://hookagency.com/website-color-schemes
