---js
const title = "Post with image";
const date = "2023-01-23";
const draft = false;
---
Here's a picture - doesn't work because of root /images issue:

![Ocean view from a beach](/images/ocean.jpg)

Try with HTML markup and force image plugin to ignore - works:

<img eleventy:ignore src="/images/ocean.jpg" alt="Ocean view from a beach" />

Try with full URL - works:

![Ocean view from a beach](http://localhost:8080/images/ocean.jpg)
