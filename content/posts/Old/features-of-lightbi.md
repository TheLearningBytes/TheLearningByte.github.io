---
title: Features of Lightbi
date: 2023-12-20
tags: ["hugo","blog"]
image : "/img/posts/img-2.jpg"
Description  : "In this blog post, I’ll walk through the key features of the Lightbi theme and how to make the most of them for a visually appealing, user-friendly website."
featured: true
---


### General
- **Three Main Content Sections:**
  - **Blog**
  - **Notes**
  - **Collections** (Newsletter)

- **Responsive Design**:
  - Built with a **mobile-first approach** for seamless viewing on any device.

- **Card-Based Theme**:
  - Flexible image placement options:
    - Image at the top of the card
    - Image in the middle of the card
    - Image at the bottom of the card
    - No image option

- **Menu Location Indicator**:
  - Clear visual cues for active menu items.

- **Multilingual Support**:
  - Includes a **language selector** for easy switching between languages.

- **Taxonomies**:
  - Organize content effectively with customizable tags and categories.

- **Search Functionality**:
  - Integrated search option for quick content access.

- **Light/Dark Theme**:
  - **Automatic theme switching** based on browser preferences.
  - Includes a manual **theme-switch button** for user control.

- **Google Analytics Integration**:
  - Track user activity with built-in support for Google Analytics.

- **SEO-Friendly**:
  - Optimized for search engines to improve visibility.

- **Commit SHA in Footer**:
  - Display the current **commit SHA** for version tracking.

- **Self-Hosted Assets**:
  - Compliant with **GDPR / EU-DSGVO** regulations by hosting all assets locally.

- **Bootstrap Icons**:
  - Beautiful, lightweight icons integrated with **Bootstrap Icons**.

### Page
- Other Posts suggestion below a post.
- Social-Media Share buttons on posts.
- Syntax highlighting.
- Cover image for each post (with Responsive image support).

### Card based theme.
To customize the image placement within a card, the Lightbi theme offers four flexible options:

- Image at the top of the card
- Image in the middle of the card
- Image at the bottom of the card
- No image

To configure this, use the `previewCardImagePlacement` parameter in the `hugo.toml` file. Set it as follows:
- For the image at the top: `previewCardImagePlacement = "top"`
- For the image in the middle: `previewCardImagePlacement = "middle"`
- For the image at the bottom: `previewCardImagePlacement = "bottom"`
- For no image: `previewCardImagePlacement = "none"`

This gives you full control over how the image is displayed in the card layout.

### What are Hugo Shortcodes?
Shortcodes in Hugo are like mini-templates that simplify embedding specialized content into a page. Hugo has built-in shortcodes, and users can create custom ones. For instance, to embed a YouTube video, instead of writing the full HTML, you can use a shortcode like `{{/*< youtube "video-id" > */}}`.

### Common Built-in Shortcodes
Here are a few popular Hugo shortcodes and how to use them:

1. **YouTube Embed**:
   
   ```
   https://www.youtube.com/watch?v=3qHkcs3kG44
   ```

   Shortcode:
   ```
   {{</* youtube 3qHkcs3kG44 */>}}
   ```
   Rendered output:
   {{< youtube 3qHkcs3kG44 >}}

   This shortcode takes a YouTube video ID, simplifying the process of embedding videos on your page.

2. **Figure**:
   Shortcode:
   ```
   {{/*< figure src="/img/posts/img-0.jpg" title="Sample Image" >*/}}
   ```

   Rendered output:
   {{< figure src="/img/posts/img-0.jpg" title="Sample Image" >}}
   
   This allows you to easily add images with captions and titles, handling image display responsively.

3. **Gist (GitHub Snippets)**:

   Shortcode:
   ```
   {{/*< gist spf13 7896402 > */}}
   ```
   Rendered:
   {{< gist spf13 7896402 >}}

   This integrates GitHub Gists by taking the username and gist ID, perfect for adding code snippets from GitHub.


   ```

4. **Twitter url**:

   ```
   https://twitter.com/binovarghese_/status/1758148486510317907
   ```

   Shortcode:
   ```
   {{</* twitter user="binovarghese_" id="1758148486510317907" */>}}
   ```

   Rendered:
   {{</* twitter user="binovarghese_" id="1758148486510317907" */>}}

### Benefits of Shortcodes
Using shortcodes in Hugo streamlines content creation and ensures consistency across pages, saving time on repeated elements and complex HTML structures. With custom shortcodes, you can build rich, interactive content while keeping Markdown files clean and easy to manage.

For more details, check out Hugo’s official [shortcode documentation](https://gohugo.io/content-management/shortcodes/).




<!--Photo by Robert Katzki on Unsplash-->
