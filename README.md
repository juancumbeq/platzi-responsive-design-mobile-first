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


<br>
<br>
<br>

# HEADER SECTION
  ## [Header Layout]()

<br>
<br>

  ## [BEM Architecture Implementation]()

<br>
<br>

  ## [Use Of ``linear-gradient``]()

<br>
<br>

  ## [Use Of ``position`` For Floating Button]()

<br>
<br>
<br>

# EXCHANGE SECTION
  ## [Base Structure Of The Exchange Section]()

<br>
<br>

  ## [Background Image]()

<br>
<br>

  ## [Currency Table Structure]()

<br>
<br>

  ## [Currency Table Base Styles]()

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
