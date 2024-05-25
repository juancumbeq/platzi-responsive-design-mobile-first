# Responsive Design: Mobile First Layout

<p align="center">
  <img src="https://img.shields.io/badge/Curso%20-Finalizado-brightgreen"/>
</p>

<br>

## What did I learn through this course:
Welcome to this course on Adaptive Design, which means mobile-first design.

Why Design for Mobile?
Over 50% of traffic comes from devices like cell phones or tablets, as it's much more convenient to open a website from a mobile device than to open a laptop and search for it. This isn't just a trend; it's a standard we must work with.

What Will You Learn in This Course?
Some of the skills you will acquire include:

Analyzing the architecture of your project starting from a wireframe
Applying styles for each breakpoint
Evaluating the quality of your design with Lighthouse
And much more!

<br>

## Demo
[Click this link to check the finished interfaces](https://juancumbeq.github.io/platzi-frontend-developer-workshop/)


<br>
<br>

# INDEX

# INITIAL SETUP
  ## ANALYZING THE DESIGN: THE COURSE PROJECT
  ## THE VALUE OF MOBILE FIRST
  ## INITIAL ARCHITECTURE
  ## ASSETS OF OUR PROJECT
  ## FONTS OF OUR PROJECT
  ## BASE STYLES

# HEADER SECTION
  ## HEADER LAYOUT
  ## BEM ARCHITECTURE IMPLEMENTATION
  ## USE OF ``LINEAR-GRADIENT``
  ## USE OF ``POSITION`` FOR FLOATING BUTTON

# EXCHANGE SECTION
  ## BASE STUCTURE OF THE EXCHANGE SECTION
  ## BACKGROUND IMAGE
  ## CURRENCY TABLE STRUCTURE
  ## CURRENCY TABLE BASE STYLES
  ## DETAILING CURRENCY TABLE STYLES
  ## FINISHING CURRENCY TABLE STYLES

# BENEFITS SECTION
  ## BASE STRUCTURE OF THE BENEFITS SECTION
  ## BENEFITS SECTION STYLES
  ## LAYOUT OF BENEFITS CARDS

# PLANS SECTION
  ## LAYOUT OF COMODIN SECTION
  ## PLANS SECTION STRUCTURE
  ## APPLYING STYLES TO THE PLANS SECTION
  ## APPLYING STYLES TO THE PLANS SECTION CARDS
  ## DETAILING STYLES ON PLAN CARDS
  ## APPLYING STYLES TO THE CALL TO ACTION BUTTON
  ## HORIZONTAL SCROLL WITH CSS

# FOOTER SECTION
  ## FOOTER

# MEDIAQUERIES
  ## APPLYING MEDIAQUERIES

# LIGHTHOUSE
  ## ANALYSIS WITH LIGHTHOUSE

# NEXT STEPS
  ## CLOSE AND NEXT STEPS

# AUTHOR



<br>
<br>
<br>

# INITIAL SETUP
  ## [Analyzing The Design: The Course Project]()
It is important to know that this course is the practical continuation of the Ultimate HTML and CSS Course.

<br>

  ### What do you need to work on your first project?
You will create a complete real project that adapts to different screen sizes. This will be a project you can add to your portfolio to showcase your skills in Web Development.

Here are some of the tools you need to use:

  - Figma: one of the most widely used software tools for building high-quality wireframes or prototypes is Figma.

Web projects are analyzed from the wireframes shared by the design team. Wireframes are prototypes that allow us to have a clear structure of what the real project will be, which we as developers will have to turn into code.

<br>

  ### Project
[The project you will build can be found here.](https://www.figma.com/proto/sMmlQaZldfDcLERYYWe6h4/Bata-Bit?node-id=44-594&scaling=scale-down)

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/batatabit.webp?raw=true" width= "100%" alt="Batatabit">
</p>

It is a static landing page with a header, a footer, and four content sections. To see how it is designed, go to the tab above and select "Open in editor."

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/open-in-editor.png?raw=true" width= "25%" alt="Open in editor">
</p>

You will be able to see all the screens created by the design team, along with the color palette, buttons, fonts, images, etc. You can also see, by clicking on a section, the CSS code that Figma recommends. It is not about copying and pasting, but about reviewing the elements that compose it to use them in our code, such as the font, color, or sizes.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/css-figma.png?raw=true" width= "75%" alt="CSS Figma">
</p>

<br>
<br>

  ## [The Value Of Mobile First]()
In responsive design, a design adapts to different views regardless of which device it was developed for first, and with this standard, we will create for mobile devices first.

<br>

  ### Who Benefits?
  * For Developers: Scaling is Easier

Converting a desktop view to a mobile view requires various considerations and can become complex as it often involves removing elements from the view, whereas it is generally easier to add them.

Mobile First, on the other hand, makes this experience more manageable, and at the code level, it is quite simple to scale from mobile to larger views, with the opportunity to add additional components in the process.

  * For Users: Less is More and for More People

Yes, it is true that more people are browsing on mobile devices. Mobile First not only reaches more devices due to the wide variety of views available on the market but also reaches more people.

Simplicity in design helps make your communication effective towards your users, providing a pleasant browsing experience and, together with an accessible design, significantly increasing your reach.

This also adds value to your users with limited connection speeds and/or low-end devices.

  * For Businesses: Better Search Engine Positioning
  
Google began working in early 2018 with an algorithm that gives greater relevance to sites optimized for mobile. This will not affect sites that have both desktop and mobile versions but will penalize those lacking a mobile alternative.

For SEO purposes, this can mean a lower user bounce rate if the content is attractive enough to retain users' attention.

<br>

  ### Progressive Evolution
Just as technology advances, we can also observe changes in frontend development trends that even become standards, such as Mobile First.

Initially, we developed for desktops where our website could be accessed from a desktop computer and laptop monitors. Then arose the need to adapt these sites to portable devices like smartphones and tablets.

As mobile site consumption increased, the need arose to develop first for these devices and then scale to larger screens. This evolution has led to some services being available as mobile-only, where the only way to access them is from a mobile device, such as financial applications, home delivery services, and more.

<br>

  ### Twitter as a Case Study
This popular social network has undergone various design transformations, one of the most important being its visualization across different devices.

By analyzing these screenshots, you can see how the mobile view remains quite simplified, and as the view size increases, other elements are added while maintaining common ones.

Mobile View (iPhone X)
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/mobileX.png?raw=true" width= "75%" alt="Mobile X">
</p>

Desktop Browser View
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/desktopX.png?raw=true" width= "75%" alt="Desktop X">
</p>

Reduced Desktop Browser View
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/reduced-desktopX.png?raw=true" width= "75%" alt="Reduced desktop x">
</p>

<br>

  ### Conclusion
Now you know why this standard is so important in your knowledge as a web developer. In addition to ensuring that your sites reach more devices and people, you are also making your code easier to scale and modify in the future.

<br>
<br>

  ## [Initial Architecture](https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/index.html)
Web architecture can be defined as the way in which the pages of a website are structured and linked to each other in a logical and coherent manner. An ideal web architecture helps users and search engines easily find what they are looking for on a website.

<br>

  ### What is the basic structure in web architecture?
  * A header with a logo, title, and a button.
  * A section with a logo, text, and a table.
  * A second section with titles, cards, text, and some icons.
  * A third section with a background image and a title.
  * A final section with cards, a title, text, and a price carousel.
  * A footer with an image and text.

Thus, we could define the basic structure of the body of our **index.html** as follows:
```
<body>
    <header></header>
    <main>
        <section></section>
        <section></section>
        <section></section>
        <section></section>
    </main>
    <footer></footer>
</body>
```

<br>

  ### Tips for Structuring Your Web Architecture
Remember:

You should have your **index.html** and **.css** files within organized folders.
**"index"** is the filename that the browser reads first.
To abbreviate the writing of HTML code, you can use Emmet. In this case, to write the basic structure, use: ``header^main>section*4^footer``

<br>
<br>

  ## [Assets Of Our Project]()
Let's learn how to download the resources or assets for a project from the prototype sent by the design team, in this case from Figma. It is important to have them ready when creating the code so that you only need to add them with the link.

<br>

  ### What are assets?
Assets are all the static resources such as images, audio, documents, and others that we will use in our project.

<br>

  ### How to download assets?
First, enter the project prototype in Figma.

  * To download any resource, click on it to see its details in the right panel.
  * Go to the "Export" tab.
  * Choose the format in which you want to download the resource, in this case, an image.
  * In the "Preview" tab, you see the final result of the resource.   *  The image to download has a transparent background.
  * Click on "Export".

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/export.webp?raw=true" width= "75%" alt="Export">
</p>

If an asset is made up of many others and you want to download it as a single file, you need to select its group.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/group-assets.webp?raw=true" width= "75%" alt="Group of assets">
</p>

When selecting the group, follow the same steps as above to export from the right panel. Don't forget to check the preview to make sure you selected the group correctly.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/group-export.webp?raw=true" width= "50%" alt="Group export">
</p>

And that's how we download all the images and other assets we need for our project. I recommend downloading images in .``svg`` format whenever possible, as this is the best format for use on the web.

Here is a link to a folder where all the assets to be used are separated into folders. [Download here](https://github.com/degranda/batata-bit).

<br>

  ### How to organize our assets?
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/assets-folder.webp?raw=true" width= "50%" alt="Assets folder">
</p>

For this case, we will create an assets folder containing two folders to distinguish which ones we will use as icons and which as images.

Rename the files so they are easy to remember, eliminating spaces to avoid conflicts with the browser when interpreting them.

<br>
<br>

  ## [Fonts Of Our Project]()
There are various types of fonts that make up the design of a project. Remember that as part of best practices in web development, you should not have more than two fonts. If you find more than two, you will need to communicate with the design team to reach a conclusion on which ones to choose.

<br>

  ### How to identify the font type in Figma
The design team may have already provided you with a report containing this information, but if not, you can identify the font from the project in Figma. To do this:

  * Click on the font to inspect.
  * In the right panel, under the inspect tab, you will see details such as size, weight, and font type. You must consider all these details when searching for them.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/figma-font.webp?raw=true" width= "75%" alt="Figma font">
</p>

This way, we check all the texts to ensure the number of fonts used.

<br>

  ### How to download fonts for a project
One of the best websites to find fonts is Google Fonts. To download the fonts for our project, follow these steps:

  * Copy the name found in the "Inspect" tab of the selected font. Click on the font.

<p align="center">
<img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/download-font.png?raw=true" width= "75%" alt="Download font">
</p>

  * You will find various font weights. Select them based on the ones found during the inspection of our project by clicking on "Select this style." Repeat these steps with the other font if you find more than one.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/font-family.webp?raw=true" width= "50%" alt="Font family">
</p>

  * Once you have selected the fonts and weights that you will use, select the "Embed" tab in the right panel. Copy the link provided by Google Fonts.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/font-embed.webp?raw=true" width= "50%" alt="Font embed">
</p>

<br>

  ### How to insert fonts in a project
To link the copied link from the previous step, open your index.html file and go to the head section. Paste the link just below the title tag.

The generated link for the project we are working on is the following:

```
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;700&family=Inter:wght@300;500&display=swap" rel="stylesheet">
```

Note: The link tag with the attribute value rel="preconnect" informs the browser that the page needs to establish a connection to another domain as quickly as possible. This way, when the browser needs to use the resources (in this case, the fonts), the resource download will be faster because the connection will already exist. This helps improve the page's performance.

Remember that Google itself indicates, right below the link it provides, how to call the font family you selected.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/css-rules.webp?raw=true" width= "50%" alt="CSS Rules">
</p>

  ### How does the ``preconnect``work?
The link tag with the attribute value rel="preconnect" informs the browser that the page needs to establish a connection to another domain as quickly as possible. This way, when the browser needs to use the resources (in this case, the fonts), the resource download will be faster because the connection will already exist.

This helps improve the page's performance. More information [here](https://css-tricks.com/using-relpreconnect-to-establish-network-connections-early-and-increase-performance/).

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/preconnect.webp?raw=true" width= "50%" alt="Preconnect">
</p>

<br>
<br>

  ## [Base Styles]()
  ### How to position content
As part of best practices, there is an order in which it is recommended to write code within CSS. This will help you keep all sections organized and know where to go back to when you need to make a change or solve a problem.

  * Positioning --> static, absolute, relative, fixed.
  * Box Model --> margin, border, padding, content.
  * Typography --> font types, sizes, etc.
  * Visual Styles --> box-shadow, border-radius, gradient, etc.
  * Others --> miscellaneous, CSS rules, and more.

<br>

  ### How to create variables
In the Branding section of the design in Figma, we can see all the colors that are used. For now, the variables we will create will be based on these colors.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/colors.webp?raw=true" width= "50%" alt="Colors">
</p>

By clicking on the adjustment icon of each color, you can view the details. Here, we have the hexadecimal code that we need.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/color-info.webp?raw=true" width= "50%" alt="Color info">
</p>

Remember, to declare a variable in CSS, we use the ``:root`` function and add a name to the variable that will contain the value we will use repeatedly in our code. Selecting all the colors, we would have:
```
:root {
    --bitcoin-orange: #f7931a;
    --soft-orange: #ffe9d5;
    --secondary-blue: #1a9af7;
    --soft-blue: #e7f5ff;
    --warm-black: #282623;
    --black: #201e1c;
    --grey: #bababa;
    --off-white: #faf8f7;
    --just-white: #fff;
}
```

<br>

  ### How to reset styles
Once the variable section is declared at the top, it is time to reset the default styles that the browser brings with the practices we already know.
```
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}
```

We will also change the font size to 62.5% to make it easier to use with REM measurements. And we will change the font style that we have embedded from Google Fonts.
```
html {
    font-size: 62.5%;
    font-family: 'DM Sans', sans-serif;
}
```

You have just applied the first styles by resetting the default ones, applying the font style, and creating the first variables of the project.

<br>
<br>
<br>

# HEADER SECTION
  ## [Header Layout]()
  ### How to layout in Figma
First, create an ``img`` tag inside the ``header`` for the logo. Then, a ``div`` container that contains:

  * ``h1`` for the main title
  * ``p`` for the paragraph
  * An ``a`` tag for the call to action, which also contains a ``span`` tag for the small icon next to it.

The code would look like this:
```
<header>
    <img src="" alt="">
    <div>
        <h1>The next revolution in cryptocurrency exchange</h1>
        <p>Batatabit helps you navigate different prices and trends.</p>
        <a href="">Check out our plans <span></span></a>
    </div>
</header>
```

The next step is to apply classes to call them from CSS and start applying styles.

<br>
<br>

  ## [BEM Architecture Implementation]()
To name the classes of containers and contents, we will use the BEM methodology

<br>

  ### What is BEM?
BEM (Block, Element, Modifier) is an agile development methodology based on components. It divides the entire interface into reusable and scalable blocks.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/bem-example.webp?raw=true" width= "100%" alt="BEM example">
</p>

This way, we can break down a section into multiple smaller sections and name them in this order and function.

<br>

  ### Tips for naming classes
  * Since there won’t be another ``img`` tag within the ``header``, we can skip adding a class and refer to it specifically.
  * The ``div`` tag is very common, so a class is necessary. We can name it ``header–title-container``, where ``header`` is the main container and ``title-container`` is the content.
  * The ``h1`` tag is unique throughout the page, so there’s no need to add a class.
  * Buttons are also common, so we apply the class ``header–button``.

Don’t Forget:
  * Set the image path in your img tag.
  * Link your .css file to your index.html before starting to apply styles.

<br>

  ### How to Apply Styles to Classes
Remember, we are designing for mobile first, so our view should focus on that. When checking the results in the browser, make sure to have the **Dimension: Responsive option enabled in the DevTools.**

  * **Header**
    * Apply ``position: relative``.
    * Use ``display: flex`` and ``flex-direction: column`` to arrange it in columns.
    * Adjust the width to 100% of the screen and the height to 334px.
    * Limit the width to a minimum of 320px.
    * Center the text with text-align: center.

```
header {
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    width: 100%;
    min-width: 324px;
    height: 334px;
    text-align: center;
}
```

  * **Img**
    * Define the dimensions of the logo with a width of 150px and a height of 24px.
    * Set the top margin to 60px.
    * Since we are using display: flex in the parent container, center the logo with align-self: center.

```
header img {
    width: 150px;
    height: 24px;
    margin-top: 60px;
    align-self: center;
}
```

  * **Div**
    * Call the container directly by the name of its class.
    * Adjust the container's width to always remain 90% between 288px and 900px. That is, it won’t grow larger than 900px or shrink smaller than 288px.
    * Set the height to 218px.
    * Add a top margin of 40px.
    * Center the text with ``text-align: center``.
    * Center the container with ``align-self: center``.

```
.header--title-container {
    width: 90%;
    min-width: 288px;
    max-width: 900px;
    height: 218px;
    margin-top: 40px;
    text-align: center;
    align-self: center;
}
```
You should be able to see our progress like this:
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/overview.webp?raw=true" width= "100%" alt="Overview">
</p>

<br>
<br>

  ## [Use Of ``linear-gradient``]()
After implementing BEM, it’s time to apply the remaining styles to the header of our project, such as the gradient background, the ``h1``, and ``p`` tags.

<br>

 ###  How to style the background
Let's go to the project prototype in Figma. By clicking on the background, we can see the colors it uses. In the CSS code section, we find a ``linear-gradient`` with the information we need. We copy it and add it to the header styles.

```background: linear-gradient(207.8deg, #201E1C 16.69%, #F7931A 100%);```

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/linear-gradient.png?raw=true" width= "100%" alt="Linear gradient">
</p>

This code shows the color percentage distribution, giving 16.69% to black and 100% to orange. When rendering it in the browser, we see that the orange occupies more space than the black, each positioned in opposite corners.

Note: If you want to create gradients easily, I recommend using CSS Gradient. It's very simple and intuitive to use.

<br>

  ### How to style the title
  * We review the main title styles in the prototype, not to copy them, but just to take details like text size and weight.

  <p align="center">
    <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/how-to-style-title.webp?raw=true" width= "100%" alt="Title">
  </p>

  * We call the ``h1`` tag using the containing class name ``.header--title-container``. While we could just call the ``h1`` tag since there should only be one in the entire document, being specific is part of good practices. As you advance, you’ll use libraries like Bootstrap that may bring styles for certain tags. By being specific, the styles we apply won’t be affected by these. Always try to be specific.

  * We adjust the font size with ``font-size: 2.4rem (24px)`` and the weight with ``font-weight: bold``.
  * We set the line height with ``line-height: 2.6rem``.
  * We change the color using the corresponding variable, ``color: var(--just-white)``.
```
.header--title-container h1 {
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--just-white);
}
```
<br>

  ### How to style the paragraph
  * We call our paragraph tag from the containing class ``.header--title-container``.

  <p align="center">
    <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/how-to-style-paragraph.png?raw=true" width= "100%" alt="Paragraph">
  </p>

  * We add a top margin to separate it from the title with ``margin-top: 25px``.
  * We adjust the size with ``font-size: 1.4rem`` and the weight with ``font-weight: 500``.
  * We give it a line height with ``line-height: 1.8rem``.
  * We change the font color using the corresponding variable, ``color: var(--soft-orange)``.

```
.header--title-container p {
    margin-top: 25px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.8rem;
    color: var(--soft-orange);
}
```

In the browser, we should see this result:

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/styled-header?raw=true" width= "100%" alt="Styled header">
</p>

<br>
<br>

  ## [Use Of ``position`` For Floating Button]()
You might have seen the button in the middle of two sections and thought: "How complicated!" But it’s not that difficult. It’s known as a floating button because it seemingly isn’t in any section but between two, giving the impression of floating in the air. The way to position it there is much simpler than it seems: by modifying its position.

<br>

  ### How to style the button
Follow these steps:

  * Call the button class from the container class with ``.header–title-container .header–button``.
  * Define its position as absolute. This makes it take the relative position of its direct parent (in this case, the header) and allows us to position the content anywhere within the container. Remember, only when the position is absolute can you add top, bottom, left, and right, because it’s fixed. This doesn’t happen if its position is relative.
  * Center it with ``left: calc(50% - 118px)``. This keeps it centered at 50%, but since the button is quite large, it subtracts 118px to the left, centering it.
  * Move the button down from the container with ``top: 270px``.
  * Add a top margin of 35px.
  * Add internal padding with ``padding: 15px``.
  * Set its width to 229px and height to 48px.
  * Give it the corresponding background color with the variable ``--off-white``.
  * Add a shadow to give it a floating effect.
  * Remove any possible default border with ``border: none``.``
  * Round the borders with ``border-radius: 5px.
Set the font size to 1.4rem and make it bold with ``font-weight: bold``.
  * Remove the underline with ``text-decoration: none`` and give it a black color with the created variable.
```
.header--title-container .header--button {
    position: absolute;
    left: calc(50% - 118px);
    top: 270px;
    display: block;
    margin-top: 35px;
    padding: 15px;
    width: 229px;
    height: 48px;
    background-color: var(--off-white);
    /* Shadow */
    box-shadow: 0px 4px 8px rgba(89, 73, 30, 0.16);
    border: none;
    border-radius: 5px;
    font-size: 1.4rem;
    font-weight: bold;
    text-decoration: none;
    color: var(--black);
}
```
It would look like this:
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/floating-button.webp?raw=true" width= "75%" alt="Floating button">
</p>

<br>

  ### How to style the icon
  * Call the span tag where we’ll create the icon from its container class with ``.header–button span``.
  * Set the display to inline-block to keep it in the same space as the accompanying text.
  * Set its width to 13px and height to 8px.
  * Add a left margin of 10px to separate it a bit horizontally from the text.
  * Call the icon file with background-image.

<br>

  ### How to call an asset from another folder
If the file you want to call is in a different folder than your .css document, you need to call the main folder.

You place ``../`` in the URL to go to the previous folder and from there find the asset. In this case, the file is in a folder within the folder where the .css file is, so we would put ``url("./assets/icons/down-arrow.svg")``.

Remember that the URL always goes in quotes.
```
.header--button span {
    display: inline-block;
    width: 13px;
    height: 8px;
    margin-left: 10px;
    background-image: url("./assets/icons/down-arrow.svg");
}
```

Our final result would look like this:
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/floating-button-arrow.png?raw=true" width= "75%" alt="Floating button arrow">
</p>

We’ve finished the header! We learned and reviewed many important functions such as positioning content with flex, defining gradients, and using calc (which can save you from many symmetrical problems).

<br>
<br>
<br>

# EXCHANGE SECTION
  ## [Base Structure Of The Exchange Section]()
We begin the second section of our project. To create it, we first need to analyze the design provided to us so we can start laying it out in our index.html. Let’s get to it!

<br>

  ### How to divide sections
First, add an identifying class to the first of the four sections we have. Using the BEM methodology, ``class="main-exchange-container"``, create the first ``div`` container inside which we will place the image. Add the class ``backgroundImg``.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/exchange-section.webp?raw=true" width= "75%" alt="Exchange section">
</p>

Create the second ``div`` container for the ``h2`` title and the ``p`` paragraph, in which we add the written content from the design. Add the class ``main-exchange-container--title``, where ``main-exchange-container`` is the block and title is the element.

The tables that show the currency values are a section by themselves, so it is more correct to create a ``section`` instead of a ``div``. Place the ``div`` inside it.
```
<section class="main-exchange-container">
    <div class="backgroundImg"></div>
    <div class="main-exchange-container--title">
        <h2>We make all exchange rates visible.</h2>
        <p>We bring real-time information from the world's most important exchanges and currencies.</p>
    </div>
    <section class="main-tables-container">
        <div></div>
    </section>
</section>
```

<br>

  ### How to style the sections
There are three elements to keep in mind:

**Main**
  * Adjust the width to 100% and the height to auto because the content we add will define the space it occupies.

  * Add ``min-width: 320px`` to prevent distortion at smaller sizes.

  * Give it a background color using the variable --off-white.
```
main {
    width: 100%;
    min-width: 320px;
    height: auto;
    background-color: var(--off-white);
}
```

**.main-exchange-container**
  * Call the first main container we are working on and similarly adjust the width to 100% and the height to auto.

  * Add padding-top: 80px and padding-bottom: 30px to add space both above and below.

  * Align the text to the center.

```
.main-exchange-container {
    width: 100%;
    height: auto;
    padding-top: 80px;
    padding-bottom: 30px;
    text-align: center;
}
```

**.main-exchange-container--title**
  * Call the container of the text section and give it a width of 90%. Limit the minimum width to 288px and the maximum to 900px.

  * Add ``margin: 0 auto`` so that, despite not occupying 100% of the width, it is always centered.
```
.main-exchange-container--title {
    width: 90%;
    min-width: 288px;
    max-width: 900px;
    margin: 0 auto;
}
```

So far, we will see this in the browser:
<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/exchange-section-overview.png?raw=true" width= "75%" alt="Exchange section overview">
</p>

<br>
<br>

  ## [Background Image]()
Now it's time to create various styles for the text section, as well as add the background image that we have in our assets. To do this, let's continue where we left off in the project's ``.css`` document.

<br>

  ### Steps to add a background image
Once you are in the project:

  * Call the ``div`` tag from the main section container.
  * First, we need to create the space it will occupy. Otherwise, we won't be able to see it. Add a width and height of 200px.
  * Center the content with ``margin: 0 auto.
  * Add a ``margin-bottom: 50px`` to give it some distance from the text.
  * Add the image with ``background-image``.
  * ``background-size: cover`` allows the image to cover the entire width while maintaining its original proportion, meaning it won't exceed the limit.
  * ``background-position: center`` ensures that we always have a view of the center of the image, regardless of the container size.
  * ``background-repeat: no-repeat`` prevents the image from repeating if it is smaller than the container.
```
.main-exchange-container .backgroundImg {
    width: 200px;
    height: 200px;
    margin: 0 auto;
    margin-bottom: 50px;
    background-image: url("./assets/img/Bitcoin.svg");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
}
```
<br>

  ### Steps to add text
Within the text, you have two important elements:

**Title**

  * Call the ``h2`` tag from the main section container.
  * Add a ``margin-bottom: 30px`` to separate it from the paragraph.
  * Adjust its size to 2.4rem and make it bold with ``font-weight: bold``.
  * Give it a line height of 2.6rem.
  * Color it with the ``--black ``variable.
```
.main-exchange-container h2 {
    margin-bottom: 30px;
    font-size: 2.4rem;
    font-weight: bold;
    line-height: 2.6rem;
    color: var(--black);
}
```

**Paragraph**

  * Call the ``p`` tag from the main section container.
  * Add a ``margin-bottom: 50px`` to give it some distance from the end of the container.
  * Adjust its size to 1.4rem and give it a weight of ``font-weight: 500``.
  * Give it a line height of 1.6rem.
  * Color it grey with ``color: #757575``. In this case, the color is not in a variable because it is used only once in the entire .css document.
```
.main-exchange-container p {
    margin-bottom: 30px;
    font-size: 1.4rem;
    font-weight: 500;
    line-height: 1.6rem;
    color: #757575;
}
```

In the browser, we will be able to see this rendered image:

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/rendered-image.webp?raw=true" width= "75%" alt="Rendered image">
</p>

<br>
<br>

  ## [Currency Table Structure]()
Let's create the code for the tables in our project. We see in the design a total of two tables.

<br>

  ### Steps to layout the table
  * Go to the section we created earlier with the class ``main-tables-container``.
  * Inside the ``div``, create a ``p`` tag for the text "Monedas".
  * Below, create another ``div`` tag that will contain the ``table`` tag, which is the table itself.
  * We work with two additional tags: ``tr`` (table row) for the rows and ``td`` (table data) for the data in each row.
  * Add the corresponding information based on the design we are working on.

```
<section class="main-tables-container">
    <div>
        <p>Monedas</p>
        <div>
            <table>
                <tr>
                    <td>Bitcoin</td>
                    <td>$1.96</td>
                </tr>
                <tr>
                    <td>Ethereum</td>
                    <td>$0.07</td>
                </tr>
                <tr>
                    <td>Ripple</td>
                    <td>$2.15</td>
                </tr>
                <tr>
                    <td>Stellar</td>
                    <td>$4.96</td>
                </tr>
            </table>
        </div>
    </div>
</section>
```
You will see that the information is organized as if it were an Excel table. Each cell occupies an equal space and is organized one below the other.

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/table.webp?raw=true" width= "50%" alt="Table">
</p>

<br>

  ### How to add classes
Start adding classes to apply styles.

  * Name the first ``div`` as ``main-currency-table`` because it is the table of current values.
  * Name the ``p`` tag as ``currency-table--title`` as the title of the container.
  * Name the ``div`` containing the table as ``currency-table--container``.
  * There is no need to add classes to the table tag or the rows, but the content does need them. For example, the first would be ``table__top-left``. We use a double underscore because, according to the BEM methodology, it differentiates an element (table) from a block and a modifier (top_left).
  * Add two classes to the price: ``table__top-right and table-right``. This is because the name column and the price column have different styles. This way, we can call a single class and apply styles to all that contain it.
  * Add the class ``table-right`` to all the ce``lls with prices in the table. For the last cell, first place the class ``table__bottom-right`` because it is the last one.
  * Add the class ``table__bottom-left`` to the last row of the table. As you can see, only the first and last rows have additional classes.
  * We only need the container where the information is updated. Create it outside the ``div`` containing the table and add a ``p`` tag for the text it contains.
  * Highlight the word shown in bold by placing it within the ``b`` tag.
  * Finally, add the class ``currency-table--date`` to the newly created container to apply styles to it.
```
<section class="main-tables-container">
    <div class="main-currency-table">
        <p class="currency-table--title">Monedas</p>
        <div class="currency-table--container">
            <table>
                <tr>
                    <td class="table__top-left">Bitcoin</td>
                    <td class="table__top-right table-right">$1.96 <span></span></td>
                </tr>
                <tr>
                    <td>Ethereum</td>
                    <td class="table-right">$0.07</td>
                </tr>
                <tr>
                    <td>Ripple</td>
                    <td class="table-right">$2.15</td>
                </tr>
                <tr>
                    <td class="table__bottom-left">Stellar</td>
                    <td class="table__bottom-right table-right">$4.96</td>
                </tr>
            </table>
        </div>
        <div class="currency-table--date">
            <p><b>Actualizado:</b> 19 de julio 23:45</p>
        </div>
    </div>
</section>
```
The rendered result in the browser would show:

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/rendered-table.webp?raw=true" width= "75%" alt="Rendered table">
</p>

<br>
<br>

  ## [Currency Table Base Styles]()
  ### Applying styles to the main container
  * First, call the class of the main table container with ``main-currency-table``.
  * Give it a width of 70% so it doesn't take up the entire space.
  * Limit the minimum width to ``235px`` and the maximum to ``500px``.
  * Set the height to ``360px``.
  * Center the content with ``margin: 0 auto``.
  * Add the font used by the tables with ``font-family: "Inter", sans-serif``.

```
.main-currency-table {
    width: 70%;
    min-width: 235px;
    max-width: 500px;
    height: 360px;
    margin: 0 auto;
    font-family: "Inter", sans-serif;
}
```

  ### Applying styles to the title
  * Instead of calling the class of the title and applying styles directly, remember we have two tables with different titles. Therefore, it's better to be specific by first calling the main table container and then the title like this: ``.main-currency-table .currency-table--title.``
  * Separate the title from the table with ``margin-bottom: 15px``.
  * Adjust the font size to ``1.8rem`` and make it ``bold``.
  * Add a line height of ``2.3rem``.

```
.main-currency-table .currency-table--title {
    margin-bottom: 15px;
    font-size: 1.8rem;
    font-weight: bold;
    line-height: 2.3rem;
    color: var(--bitcoin-orange);
}
```

  ### Applying styles directly to the container
  * Call the ``div`` containing the table with ``.currency-table--container``.
  * Give it a width of ``90%`` of its parent container.
  * Set a minimum width of ``230px`` and a maximum of ``300px``.
  * Adjust the height to ``250px``.
  * Center the content with ``margin: 0 auto``.

```
.currency-table--container {
    width: 90%;
    min-width: 230px;
    max-width: 300px;
    height: 250px;
    margin: 0 auto;
}
```
  ### Applying styles to the table
  * Call the ``table`` tag from its parent container with ``.currency-table--container table``.
  * Give it a width and height of ``100%`` to occupy the entire space of the parent container.

```
.currency-table--container table {
    width: 100%;
    height: 100%;
}
```
  ### Applying styles to the cells
  * Call the ``td`` tag from its parent container with ``.currency-table--container td``.
  * Give it a width of ``50%`` as they take up half the space of the rows.
  * Adjust the font size to ``1.6rem`` and set the weight to ``500``.
  * Add a line height of ``1.9rem``.
  * Change the color using the ``--grey variable``.
  * Add a background color using the ``--just-white`` variable.

```
.currency-table--container td {
    width: 50%;
    font-size: 1.6rem;``
    font-weight: 500;
    line-height: 1.9rem;
    color: var(--grey);
    background-color: var(--just-white);
}
```
This would be our final result:

<p align="center">
  <img src="https://github.com/juancumbeq/platzi-responsive-design-mobile-first/blob/main/readme_images/final-table.webp?raw=true" width= "75%" alt="Final table">
</p>

<br>
<br>

  ## [Detailing Currency Table Styles]()

<br>
<br>

  ## [Finishing Currency Table Styles]()

<br>
<br>
<br>

# BENEFITS SECTION
  ## [Base Structure Of The Benefits Section]()

<br>
<br>

  ## [Benefits Section Styles]()

<br>
<br>

  ## [Layout Of Benefits Cards]()

<br>
<br>
<br>

# PLANS SECTION
  ## [Layout Of Comodin Section]()

<br>
<br>

  ## [Plans Section Structure]()

<br>
<br>

  ## [Applying Styles To The Plans Section]()

<br>
<br>

  ## [Applying Styles To The Plans Section Cards]()

<br>
<br>

  ## [Detailing Styles On Plan Cards]()

<br>
<br>

  ## [Applying Styles To The Call To Action Button]()

<br>
<br>

  ## [Horizontal Scroll With CSS]()

<br>
<br>
<br>

# FOOTER SECTION
  ## [Footer]()

<br>
<br>
<br>

# MEDIAQUERIES
  ## [Applying Mediaqueries]()

<br>
<br>
<br>

# LIGHTHOUSE
  ## [Analysis With Lighthouse]()

<br>
<br>
<br>

# NEXT STEPS
  ## [Close And Next Steps]()

<br>
<br>
<br>

# AUTHOR
