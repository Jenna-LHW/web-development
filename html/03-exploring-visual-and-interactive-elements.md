# Exploring Visual and Interactive Elements
## Images
### The `<img>` Tag and Its Attributes
The`<img>` tag is an empty element which means that it does not have a closing tag.

The `src` attribute specifies the source of URL of the image that should be displayed.  
For example: `src="https://edube.org/uploads/media/default/0001/03/mountain_landscape.jpg"`  

The `alt` attribute specifies the width of the image. It can be defined in pixels (eg, `width="340"`) or as a percentage of the containing element's width (eg, `width="50%"`).

The `height` attribute specifies the height of the image in pixels or as a percentage of its parent container.  
For example: `height="250"` or `height="50%"`.

Example of the `<img>` tag with all the four attributes in action:
```HTML
<img src="https://edube.org/uploads/media/default/0001/03/mountain_landscape.jpg" alt="Mountain landscape" width="340" height="250">
```
Output:  
<img src="https://edube.org/uploads/media/default/0001/03/mountain_landscape.jpg" alt="Mountain landscape" width="340" height="250">

### Image Formats
The most common image formats used on the web are:
- JPEG (Joint Photographic Experts Group) best suited for for photographs or images with many colours and gradients. JPEG imagages are compressed, which means that they have a smaller file size but the compression can result in a loss quality.
- PNG (Portable Network Graphics) best suited for imgaes with transparent backgrounds or imaged with sharp edges, such as logos or graphics. PNG images are lossless, which means that they do not lose quality when compressed.
- GIF (Graphics Interchange Format) best suited for simple animated graphics or images with limited colours, such as icons or buttons. GIF images can also be used to create simple animations
- SVG (Scalable Vector Graphics) is ideal for images that need to be scaled without losing quality

> To check  compatibility with different web browser you use this:
> <a href="https://caniuse.com/" target="_blank">caniuse.com</a>


### Image Location
When adding images, it's important to consider the location of the image file. If the image is stored locally (oon your computer), it will need to be uploaded to the website's server.

#### Relative Path
A relative path is a path that starts from the directory of the HTML file. For example:
```HTML
<img src="images/pictures.jpg" alt="A picture">
```
#### Absolute Path
An absolute path is a path that starts from the root directory of the website. For example:
```HTML
<img src="https://example.com/images/picture.jpg" alt="A picture">
```

### Responsive Images
To create responsive images in HTML, you can use

#### The `srcset` Attribute
The `scrcet` attribute allows you to specify a list of images files with different resolutions, sizes and formats. When the browser loads the image, it will select the most appropriate image from the list based on the screen size and the device's capabilities.

#### The `sizes` Attribute 
The `sizes` attribute specifies the size of the image container in which the image will be displayed. In other words, it tells the browser how much screen spave the image will occupy on different devices.

Example:
```HTML
<img src=sunflowers.jpg"
     alt="Sunflowers in the sunset"
     srcset="sunflowers-small.jpg 480w,
             sunflowers-medium.jpg 800w,
             sunflowers-large.jpg 1200w"
     sizes="(max-width: 480px) 95vw,
            (max-width: 800px) 45vw,
            30vw">
```
So, what happens here?

- The code sets the source of the image to `sunflowers.jpg`,
- The `alt` attribute provides the following alternative text for the image: “Sunflowers in the sunset”,
- The `srcset` attribute provides three different versions of the image with different sizes and resolutions (480, 800, and 1200 pixels wide),
- The `sizes` attribute defines the width of the image at different breakpoints. In our example the image will take up to 95% of the viewport width if the viewport is less than 480px, 45% if the viewport is between 480px and 800px wide, and 30% if the viewport is larger than 800px.

> Note:
> - For phone: `max-width: 480px`
> - For tablet: `max-width: 800px`
> - For laptop/pc: greater than 800px

### Other Image-Specific Attributes
#### The `border` attributes 
The `border` attributes specifies the width of the border around the image.
```HTML
<img src="example.jpg" alt="Example image" border="2">
```

#### The `haspace` and `vspace` Attributes
The `haspace` and `vspace` attributes specify the horizontal and vertical space around the image, respectively. 
```HTML
<img src="example.jpg" alt="Example image" hspace="10" vspace="10">
```

#### The `align` Attributes
The `align` Attributes allows for specifying the alignment of an image relative to surrounding content, with values like `left`, `right` and `center`.
```HTML
<img src="example.jpg" alt="Example image" align="left">
```

> Note:
> While these attributes provide straight forward ways to adjust image presentation, modern HTML practices use CSS to achieve these effects. 

## Hyperlinks
