---
layout: Responsive Images
title: Why We Need Them
---
 
 
## We need Responsive Images because...  

### Using CSS to implement responsive images:
Put this code into the head of your document in a style tag

```
.site-banner {
  width: 300px;
  height: 100px;
  background-image: url('images/site-banner-mobile.jpg');
}

@media (min-width: 480px) {
  .site-banner {
    width: 440px;
    height: 200px;
    background-image: url('images/site-banner-mobile-wide.jpg');
  }
}

@media (min-width: 768px) {
  .site-banner {
    width: 720px;
    height: 250px;
    background-image: url('images/site-banner-tablet.jpg');
  }
}

@media (min-width: 1024px) {
  .site-banner {
    width: 1000px;
    height: 300px;
    background-image: url('images/site-banner-desktop.jpg');
  }
}

```



#### Using Picturefill to implement responsive images:  

Add these two elements to the head of your document:

```
<script>
// Picture element HTML5 shiv
document.createElement("picture");
</script>

```

and

```
<script src="picturefill.js" async></script>

```
 

