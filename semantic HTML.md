Main Method:

```html
<html>
  <head> </head>
  <body>
    <header>// logo & navigation here</header>
    <nav>// nav links here</nav>
    <main>// content here (section/article/form)</main>
    <footer>// info here (copyright/FAQ)</footer>
  </body>
</html>
```

Detailed Method:

```html
<html>
  <head>
    <title>My Blog Post</title>
  </head>
  <body>
    <header>
      <h1>My Blog</h1>
      <nav>
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <article>
        <h2>My Blog Post</h2>
        <p>This is the main content of my blog post.</p>
        <ul>
          <li>List item 1</li>
          <li>List item 2</li>
          <li>List item 3</li>
        </ul>
        <blockquote>
          <p>This is a quote from another source.</p>
          <cite>Source Name</cite>
        </blockquote>
        <figure>
          <img src="image.jpg" alt="An image related to the blog post" />
          <figcaption>This is a caption for the image.</figcaption>
        </figure>
      </article>
    </main>

    <aside>
      <h3>Related Posts</h3>
      <ul>
        <li><a href="#">Post 1</a></li>
        <li><a href="#">Post 2</a></li>
        <li><a href="#">Post 3</a></li>
      </ul>
    </aside>

    <footer>
      <p>Copyright &copy; 2023 Your Name or Company Name. All rights reserved.</p>
    </footer>
  </body>
</html>
```
