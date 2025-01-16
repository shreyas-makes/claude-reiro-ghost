Webmentions for Ghost: POSSE Implementation Guide 🌐
A complete solution for implementing POSSE (Publish Own Site, Syndicate Elsewhere) on Ghost blogs using webmentions. Transform your Ghost blog into a hub of distributed conversations while maintaining digital sovereignty.
The Challenge 🤔
Modern web publishing faces a paradox: we need social media's reach but want independence in our content. This implementation solves that by:

Replacing Ghost's native comments with webmentions
Connecting your blog to the broader social web
Maintaining your content's sovereignty while enabling distributed discussions

## Features ✨

1. Webmention Support: Full implementation of webmention.io integration
2. Brid.gy Integration: Connect with Mastodon, Bluesky, and other platforms
3. URL Handling: Works with both www and non-www domain variants
4. Custom Styling: Clean, professional design that matches Ghost's aesthetic
5. Comment Replacement: Complete replacement for Ghost's native commenting system

## Installation 🛠️

1. Code Injection Setup
Add this to your Ghost Admin → Settings → Code injection → Site Header:

```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/prismjs/themes/prism-twlight.min.css">
<link rel="microsub" href="https://aperture.p3k.io/microsub/1003">
<link rel="authorization_endpoint" href="https://indieauth.com/auth">
<link rel="token_endpoint" href="https://tokens.indieauth.com/token">
<link rel="me" href="https://github.com/shreyas-makes">

<link rel="webmention" href="https://webmention.io/www.shreyasprakash.com/webmention">
<link rel="pingback" href="https://webmention.io/www.shreyasprakash.com/xmlrpc">

<!-- <link rel="webmention" href="https://webmention.io/shreyasprakash.com/webmention">
<link rel="pingback" href="https://webmention.io/shreyasprakash.com/xmlrpc"> -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/bigfoot/2.1.4/bigfoot-default.css" integrity="sha512-DhI5L06RHGX5gUnHM2t7ikxNvKfyb+C2/0coMbHOg6iep7cX35PNUmOBwLz9RBvCVllR3mjX7kHnEDR4xQcqlA==" crossorigin="anonymous" referrerpolicy="no-referrer" />

<style>
  /* Container */
.wm-container {
    background: var(--color-four);
    border-radius: var(--border-radius);
    box-shadow: 0 4px 12px var(--opacity-four);
    padding: 2.5rem;
    margin: 4rem 0 6rem;
}

/* Header */
.wm-header {
    font-family: var(--font-family-one);
    font-size: 2.8rem;
    font-weight: var(--font-weight-one-bold);
    color: var(--color-font-one);
    margin-bottom: 2rem;
}

/* Likes and Retweets Section */
.wm-avatar-grid {
    display: flex;
    align-items: center;
    padding-bottom: 2rem;
    margin-bottom: 2rem;
    border-bottom: var(--border) var(--color-border-one);
}

.wm-avatar-grid .wm-avatar-link {
    width: 40px;
    height: 40px;
    margin-right: -10px;
    position: relative;
    z-index: 1;
}

.wm-avatar-grid .wm-avatar-img {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    border: 2px solid var(--color-four);
    object-fit: cover;
}

.wm-reactions-count {
    font-size: 1.6rem;
    color: var(--color-font-one);
    margin-left: 1.5rem;
}

/* Comments Section */
.wm-mention-item {
    display: grid;
    grid-template-columns: 40px 1fr;
    gap: 15px;
    padding: 20px 0;
    border-bottom: var(--border) var(--color-border-one);
}

.wm-mention-item:last-child {
    border-bottom: none;
}

/* Author Image */
.wm-author-img {
    width: 40px;
    height: 40px;
    border-radius: 50%;
    object-fit: cover;
}

/* Content Container */
.wm-mention-content-wrapper {
    display: flex;
    flex-direction: column;
    gap: 12px;
}

/* Author Name */
.wm-author-name {
    font-size: 1.6rem;
    font-weight: var(--font-weight-three-bold);
    color: var(--color-font-one);
    text-decoration: underline;
}

/* Content */
.wm-mention-content {
    font-size: 1.6rem;
    color: var(--color-font-one);
    line-height: 1.5;
}

/* Source and Date Line */
.wm-mention-source-line {
    font-size: 1.6rem;
    color: var(--color-font-two);
}

.wm-mention-source {
    color: var(--ghost-accent-color);
    text-decoration: underline;
}

.wm-mention-metadata {
  font-size: 1.6rem;
}
  


</style>
<script src="/assets/js/webmention.js" async></script>

<script src="https://cdn.jsdelivr.net/npm/prismjs/prism.min.js" defer></script>
<script src="https://cdn.jsdelivr.net/npm/prismjs/plugins/autoloader/prism-autoloader.min.js" defer></script>

<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-LKDSFYXM8M"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-LKDSFYXM8M');
</script>

```

## File Structure

```
plaintextCopyassets/
└── js/
    └── webmention.js    # Webmention handler
post.hbs                 # Modified template
```

## Brid.gy Configuration

1. Visit brid.gy
2. Connect desired platforms: Mastodon, Bluesky
3. Store Micropub tokens securely

## Usage 📝

1. Publish content on your Ghost blog
2. Content syndicates to connected platforms via Brid.gy
3. Social interactions flow back as webmentions
4. Conversations appear on your original post

## Troubleshooting 🔧

Common issues and solutions:

1. No webmentions showing: Verify webmention.io endpoint configuration
2. URL mismatches: Check URL handling in fetchWebmentions function
3. Style conflicts: Review CSS specificity
4. Brid.gy issues: Validate Micropub token status

## Contributing 🤝

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## Acknowledgments 🙏

1. webmention.io for the webmention infrastructure
2. Brid.gy for social platform integration
3. Ghost for the blogging platform
4. IndieWeb community for POSSE principles
