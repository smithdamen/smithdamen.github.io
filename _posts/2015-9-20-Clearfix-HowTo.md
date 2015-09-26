# How-To Get Out Of CSS Layout Hell

### CSS clearfixes made simple and quick

If you're like me, you might prefer to use CSS floats to create the layout for your websites. Until I started doing some research online, I had no idea how to get all of my content to fit properly in their parent containers. I kept hearing about clearfixes and noticed them being added to the code for a Bootstrap project I was working on.

```html

  Example:
  
  <div class="container">
    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>
    <div class="box"></div>
  </div>
  
```
  
This is a bit of HTML with 4 boxes inside a containing <div>. Within these boxes we can have any sort of content.

```css
  
  .container {
    width: 100%;
  }
  
  .box {
    width: 200px;
    height: 200px;
    float: left;
  }
  
```
  
The "container" <div> will not size itself to fit the floated elements within and will throw off the layout of the rest of the page.

```css
  
  CSS with clearfix:
  
  .container {
    width: 100%;
  }
  
  .container:after {
    clear: both;
    content: " ";
    display: table;
  }
  
  .box {
    width: 200px;
    height: 200px;
    float: left;
  }
  
```
Once this has been applied to your container, it will take up the proper amount of height and prevent content beneath this section from overlapping.

### SASS Mixin

I recently learned how to make SASS mixins and have started making little shortcuts as I continue to work on my web projects. I recently made a mixin that allows me to add a clearfix to any container with one line of code.

```css

  @mixin clearfix {
    &:after {
      clear: both;
      content: " ";
      display: table;
    }
  }
  
```

This would be your scss clearfix mixin that you can import into your layout stylesheet. Applying this mixin in a SASS file is incredibly easy.

```css

  @import 'clearfix'
  
  .container
    width: 100%
    +clearfix
  
  .box
    width: 200px
    height: 200px
    float: left
    
```

I hope this helps with some if your projects. [Click to learn more about SASS and Mixins](http://sass-lang.com/guide)