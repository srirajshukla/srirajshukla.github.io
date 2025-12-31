# Blog System

This is a simple, no-build blog system using pure HTML and CSS.

## How to Write a New Blog Post

### 1. Create a new HTML file in `blog/posts/`

Use this template for your blog post:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Post Title - Gyanendra Shukla</title>
    <link rel="stylesheet" href="../../styles.css">
</head>
<body>
    <div class="grid-bg"></div>

    <div class="container">
        <header class="page-header">
            <h1><a href="/">Gyanendra Shukla</a></h1>
            <nav class="nav-links">
                <a href="/#projects">Projects</a>
                <a href="/#reading">Reading</a>
                <a href="/blog">Blog</a>
                <a href="/contact">Contact</a>
            </nav>
        </header>

        <article class="blog-post">
            <header class="blog-post-header">
                <h1 class="blog-post-title">Your Post Title</h1>
                <div class="blog-post-meta">
                    <span class="post-date">Month Day, Year</span>
                    <div class="post-tags">
                        <span class="tag">Tag1</span>
                        <span class="tag">Tag2</span>
                    </div>
                </div>
            </header>

            <div class="blog-post-content">
                <!-- Your blog content goes here -->
                <p>Your introduction paragraph...</p>

                <h2>Section Title</h2>
                <p>Section content...</p>

                <h3>Subsection</h3>
                <p>More content...</p>

                <!-- Code blocks -->
                <pre><code>your code here</code></pre>

                <!-- Inline code -->
                <p>Use <code>inline code</code> like this.</p>

                <!-- Lists -->
                <ul>
                    <li>Item 1</li>
                    <li>Item 2</li>
                </ul>

                <!-- Blockquotes -->
                <blockquote>
                    <p>A quote or important note</p>
                </blockquote>

                <!-- Links -->
                <p>Check out <a href="https://example.com">this link</a>.</p>
            </div>
        </article>

        <footer>
            <p>© 2025 Gyanendra Shukla</p>
        </footer>
    </div>
</body>
</html>
```

### 2. Add the post to the blog listing page

Edit `blog/index.html` and add your post preview in the `<div class="blog-posts">` section:

```html
<article class="blog-post-preview">
    <div class="post-date">YYYY-MM-DD</div>
    <h3><a href="/blog/posts/your-post-filename.html">Your Post Title</a></h3>
    <p class="post-excerpt">A brief 1-2 sentence description of your post.</p>
    <div class="post-tags">
        <span class="tag">Tag1</span>
        <span class="tag">Tag2</span>
    </div>
</article>
```

Add new posts at the **top** of the list so the most recent posts appear first.

## Typography Guidelines

The blog styling is optimized for readability:

- **Max width**: 720px for comfortable reading line length
- **Font size**: 1.125em (18px) for body text
- **Line height**: 1.8 for comfortable reading
- **Headings**: Use h2 for main sections, h3 for subsections
- **Code blocks**: Dark background with light text, syntax highlighting ready

## Styling Elements

### Headings
- `h2` - Major sections (1.8em)
- `h3` - Subsections (1.4em)

### Code
- Inline code: `<code>text</code>`
- Code blocks: `<pre><code>text</code></pre>`

### Lists
- Unordered: `<ul><li>...</li></ul>`
- Ordered: `<ol><li>...</li></ol>`

### Quotes
- `<blockquote><p>...</p></blockquote>`

### Links
- Styled with underline on hover
- `<a href="...">text</a>`

## Tips

1. Keep paragraphs focused (3-5 sentences)
2. Use headings to break up long content
3. Add code blocks for technical content
4. Use lists for step-by-step instructions
5. Include relevant tags for categorization
6. Write a clear, concise excerpt (1-2 sentences)

## File Naming

Use kebab-case for filenames: `my-blog-post-title.html`
