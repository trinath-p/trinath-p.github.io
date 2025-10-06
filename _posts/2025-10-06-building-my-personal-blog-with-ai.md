---
title: "Building My Personal Blog: A Journey from Idea to Deployment"
date: 2025-10-06 10:00:00 +0000
categories: [Web Development, My Blog Website]
tags: [github-pages, jekyll, giscus, analytics, seo]
toc: true
---


After years of working in clinical data standards and Python development, I realized I had accumulated a wealth of knowledge and experiences that could benefit others in the field. The idea of sharing my insights, tutorials, and industry observations through a personal blog had been brewing in my mind for months. Finally, in late 2025, I decided to take the plunge and build my own corner of the internet. Mainly I solved my biggest nightmare, a full markdown supported + GitHub integration system.

## Choosing the Right Technology Stack

### Why Jekyll + GitHub Pages?

When it came to choosing the foundation for my blog, I had several options to consider:

- **Wix**: Best for portfolio and normal blogging (I have my portfolio in wix)
- **WordPress**: Feature-rich but felt overkill for a personal blog
- **Medium/Dev.to**: Easy to use but lacked customization
- **Jekyll + GitHub Pages**: Perfect balance of simplicity and full control + markdown support (In these years i am loving Markdown language more than Python and SAS)

I chose Jekyll with GitHub Pages because:

1. **Free hosting** - No monthly costs to worry about
2. **Version control** - My entire blog is a Git repository
3. **Fast loading** - Static site generation means lightning-fast performance
4. **SEO-friendly** - Clean URLs and meta tags out of the box
5. **Developer-friendly** - Write posts in Markdown, deploy with Git

### The Chirpy Theme: A Perfect Match

After researching Jekyll themes, I stumbled upon the **Chirpy** theme, which immediately caught my attention. Its clean design, excellent typography, and built-in features like:

- Dark/light mode toggle
- Table of contents
- Tag and category pages
- Search functionality
- Social media integration

It felt like the perfect foundation for a professional developer blog.

## The Development Process: Step by Step

### 1. Setting Up the Foundation

The initial setup was surprisingly straightforward:

```bash
# Clone the Chirpy theme
git clone https://github.com/cotes2020/jekyll-theme-chirpy.git my-blog
cd my-blog
bundle install
bundle exec jekyll serve
```

Within minutes, I had a fully functional blog running locally at `localhost:4000`.

### 2. Customizing the Configuration

The `_config.yml` file became my command center. I customized the site title, description, URL, and added my social media links. I also set up my timezone and other personal details to make the blog truly mine. This configuration file controls everything from the site's appearance to its SEO settings.

### 3. Adding Analytics and SEO

Understanding my audience and optimizing for search engines were crucial goals. I integrated:

**Google Analytics 4**: To track visitor behavior and popular content. I added my tracking ID to the configuration file, which automatically includes the Google Analytics script on every page.

**Google Search Console**: For SEO monitoring and sitemap submission. I submitted the automatically generated sitemap, requested indexing for key pages, and set up performance monitoring to track how my content performs in search results.

### 4. Implementing Comments with Giscus

Engagement was important to me, so I added a commenting system. After evaluating options:

- **Disqus**: Popular but privacy concerns
- **Utterances**: GitHub Issues-based, good but limited
- **Giscus**: GitHub Discussions-based, perfect for developers

I chose Giscus because:
- It's privacy-friendly (no tracking)
- Integrates seamlessly with GitHub
- Spam-resistant (requires GitHub account)
- Free and open-source

The setup involved enabling GitHub Discussions on my repository and configuring the integration in my site's configuration file with the repository details and discussion category settings.

## Challenges and Solutions

### The Sitemap Issue

One interesting challenge I encountered was with the sitemap generation. Initially, my local development environment was generating sitemaps with `localhost:4000` URLs instead of the production domain. This caused Google Search Console to fail when fetching the sitemap.

**Solution**: The issue resolved itself when I deployed to GitHub Pages, as the production build correctly generated URLs with the proper domain. This taught me the importance of testing in a production-like environment.


## Lessons Learned

### What Worked Well

1. **Choosing the right theme** - Chirpy provided everything I needed out of the box
2. **Starting simple** - Focus on content first, features later
3. **Using Git** - Version control for my entire blog is invaluable
4. **Free tools** - GitHub Pages + Jekyll + Giscus = $0 hosting cost

## The Role of AI and Cursor in This Process

I'll be transparent: AI and modern development tools played a significant role in this blog's creation. I used **Cursor**, an AI-powered code editor, throughout the entire development process. This powerful combination helped me:

- **Technical troubleshooting** - Solving configuration issues and debugging problems
- **Learning new technologies** - Understanding Jekyll, GitHub Pages, and web development concepts
- **Code generation and optimization** - Writing configuration files and implementing features
- **Real-time guidance** - Getting instant help with technical decisions

The AI-powered development environment didn't replace my expertise or creativity—it amplified them. It helped me focus on what matters most: creating valuable content for my readers while learning and building efficiently. This represents the future of web development, where human creativity is enhanced by intelligent tools.

## Technical Stack Summary

For those interested in the technical details:

- **Framework**: Jekyll (Ruby-based static site generator)
- **Theme**: Chirpy v7.3+
- **Hosting**: GitHub Pages
- **Analytics**: Google Analytics 4
- **SEO**: Google Search Console
- **Comments**: Giscus (GitHub Discussions)
- **Version Control**: Git + GitHub
- **Domain**: trinathpanda.github.io (GitHub Pages subdomain)

## Conclusion

Building this blog has been an incredibly rewarding experience. It's taught me that creating a professional online presence doesn't require expensive tools or complex setups. With the right combination of free technologies and a clear vision, anyone can build a platform to share their knowledge and connect with like-minded professionals.

The journey from idea to deployment took dedication, but the result is a fast, SEO-optimized, and engaging blog that truly represents my professional identity. Most importantly, it's a platform that will grow with me as I continue to learn and share in the field of clinical data standards and Python development.

If you're considering starting your own blog, my advice is simple: start with a solid foundation (like Jekyll + GitHub Pages), focus on creating valuable content, and don't be afraid to leverage modern tools (including AI) to amplify your capabilities.

The web is built by sharing knowledge—and now I'm proud to be part of that tradition.

---

*Have questions about building your own blog? Feel free to leave a comment below or connect with me on [LinkedIn](https://www.linkedin.com/in/trinath-panda). I'd love to hear about your blogging journey!*
