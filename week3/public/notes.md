1. In JGPFpage26 week 3 Set up folder structure and upload assets. CSS/JS/ assets
2. start htmlf page ! index.html

   CTRL sift + make text bigger on VSC

3. Add links for bootstrap

    Show [bootstrap blog](https://blog.getbootstrap.com/)

    Show [bootstrap cheatsheet themeselection](https://bootstrap-cheatsheet.themeselection.com/)

    Show [bootstrap cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/  )

    Follow [introduction](https://getbootstrap.com/docs/5.3/getting-started/introduction/)
    place both link and script after the title.

4. Add a div with h1 and p show page is not responsive.

    [py-5 sets spacing above and below](https://getbootstrap.com/docs/5.0/utilities/spacing/)

    [text-start left aligns text](https://getbootstrap.com/docs/5.0/utilities/text/)

    [containers](https://getbootstrap.com/docs/5.0/layout/containers/)

    Compare:
    ```html
    <div class="container-sm text-start text-sm-center" style="background-color: aquamarine;">
    ```
    with

    <div class="container-fluid text-start text-sm-center" style="background-color: aquamarine;">

    Pull the page off browser to separate small window.

    Look for containers on bootstrap intro

5. [Try out a blockquote](https://bootstrap-cheatsheet.themeselection.com/)
6. [Try out typography display](https://bootstrap-cheatsheet.themeselection.com/)

    Set <h1> to display-5
    [Try out fw font weight in Utility Text](https://bootstrap-cheatsheet.themeselection.com/)
    Set <h1> to fw-bold

7. [try out columns](https://getbootstrap.com/docs/5.3/layout/columns/)

    This is a 12 colum model so col-4 covers a third of the available width,
    col-6 covers half width.  Total of colums should add up to 12.

    [Try out col-md snippet](https://bootstrap-cheatsheet.themeselection.com/) 
   
8. [try out font size fs](https://bootstrap-cheatsheet.themeselection.com/) 

9. Clean up and break video there.

-----------------------

# making demo page

```html
<div class = "container-fluid py-5 text-start text-sm-center" >
<h1 class=" display-5 fw-bold" >My first Bootstrap page</h1>
<p class="col-md-8 fs-4">Resize this responsive page to see the effect</p>
</div>
```

1. Add navigation bar

    [Navbar](https://getbootstrap.com/docs/5.3/components/navbar/)

    Add navbar with image and text

    Add list free navlinks
    Home Design Play Game Disabled 

   add navbar-expand-lg to make hamburger break to full menu.

2. Look at color schemes and go for dark border

3. Add a [drop down button link ](https://getbootstrap.com/docs/5.3/components/dropdowns/)   

```html
         <span class="nav-item dropdown" >
            <a class="nav-link dropdown-toggle" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">
                3D Scenes
            </a>
          <ul class="dropdown-menu" >
            <li><a class="dropdown-item" href="element1/index.html" >Scene 1</a></li>
            <li><a class="dropdown-item" href="element1/index.html">Scene 2</a></li>
            <li><a class="dropdown-item" href="element1/index.html">Scene 3</a></li>
            <li><a class="dropdown-item" href="element1/index.html">Scene 4</a></li>
            <li><hr class="dropdown-divider"></li>
            <li><a class="dropdown-item" href="element1/index.html">Scene 5</a></li>
          </ul>
        </span>
```

End of part 1

Look back at lab sheet - next section is a 3 columd div to display text about games.

1. Make a div

```html
<div class = "container-fluid mt-3"></div>
```
Add a single row

```html
<div class = "container-fluid mt-3">
    <div class = "row"></div>
</div>
```
Add three columns each 4 (of 12) grid spaces wide.

```html
<div class = "container-fluid mt-3">
    <div class = "row">
        <div class = "col-sm-4"></div>
        <div class = "col-sm-4"></div>
        <div class = "col-sm-4"></div>
    </div>
</div>
```

2. Grab some placeholder test from a [lorem ipsum generator](https://www.lipsum.com/). 

Lorem ipsum dolor sit amet, consectetur adipiscing elit. In congue, enim ut aliquam mattis, risus libero porta est, et imperdiet sapien sapien sit amet nulla. Pellentesque suscipit quis nisi eget finibus. Nullam facilisis eros ut ultricies cursus. Vestibulum consectetur egestas magna, in lobortis mauris ultricies at. Cras sit amet felis auctor, euismod leo quis, aliquet ex. In ut bibendum turpis, nec varius libero. Donec id accumsan mauris, id pulvinar erat. Fusce luctus enim sed nisi tempus convallis. In sed dapibus ante, consequat pellentesque felis. Quisque erat quam, pharetra ac imperdiet non, posuere in turpis. In ornare scelerisque arcu, quis finibus augue scelerisque ac. Nullam quis tempus sapien, non molestie mauris. Cras pellentesque ex libero.

Donec porttitor mauris sit amet est vestibulum posuere. Aliquam sit amet massa vitae orci semper lobortis vitae et libero. Ut sagittis venenatis imperdiet. Cras ut lacinia enim, nec efficitur enim. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aliquam at elementum diam. Cras volutpat sit amet nisl nec volutpat. Vestibulum at odio orci. Sed quis blandit urna. Aliquam id volutpat erat. 

3. Add header and some text to each column and check that the page is responsive.

4. Add a [carousel component](https://getbootstrap.com/docs/5.0/components/carousel/#with-captions) to display 3 images.

Copy from Captions section.

Add images Fortnight, ratchetandclank and splatoon.

```html
       <h5 style = "background-color: black;">Fortnite</h5>
       <p style = "background-color: black;">A game by Epic Games!.</p>

        <h3 style = "background-color: black;">Ratchet & Clank</h5>
        <p style = "background-color: black;">A game by insomniac games!</p>

        <h3 style = "background-color: black;">TSplatoon 3</h5>
        <p style = "background-color: black;">A game by Nintendo.</p>
```

5. Try adding a [card](https://getbootstrap.com/docs/5.0/components/card/#example)

Use a basic card.

```html
<div class="card" style="width: 18rem;">
  <img src="assets/icon.jpg" class="card-img-top" alt="Icon">
  <div class="card-body">
    <h5 class="card-title">Derek Turner</h5>
    <p class="card-text">Derek is a Senior Lecturer at UWS specialising in Music Technology, Computer Games and Internet Technologies.</p>
    <a href="https://bbc.co.uk" class="btn btn-primary">Go to BBC</a>
  </div>
</div>
```

6.  Add an [Accordian]
        
   1. What is HTML?

   HTML stands for HyperText Markup Language. HTML is the standard markup language for describing the structure of web pages. 

   ``` html
    <a href="https://www.tutorialrepublic.com/html-tutorial/" target="_blank">Learn more.</a> 
   ```

    2. What is Bootstrap?

    Bootstrap is a sleek, intuitive, and powerful front-end framework for faster and easier web development. It is a  collection of HTML and CSS conventions.

   ``` html
    <a href="https://www.tutorialrepublic.com/twitter-bootstrap-tutorial/" target="_blank"> 
   ```

   3. What is CSS?

    CSS stands for Cascading Stylesheets. Allows you to specify properties for a sected HTML element such as colours and backgrounds

       ``` html
    <a href="https://www.tutorialrepublic.com/css-tutorial/" target="_blank"> 
   ```

4. Reach back to week 1 and add 5 versions of the test card to week 3.


