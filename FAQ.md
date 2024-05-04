# Frequently Asked Questions (FAQ) for Hugo

Welcome to the FAQ section for Hugo! Below you'll find answers to common questions related to using Hugo as your static site generator.

## Getting Started with Hugo

### What is Hugo?
Hugo is a fast and flexible static site generator, ideal for building websites from plain text into beautiful, fast websites and blogs.

### How do I install Hugo?
- **macOS:** Use Homebrew: `brew install hugo`
- **Windows:** Use Chocolatey: `choco install hugo`
- For other systems, download from the [Hugo Releases](https://github.com/gohugoio/hugo/releases) page.

### How do I create a new site?
Create a new site with `hugo new site [site-name]`, which sets up the necessary folder structure.

## Working with Content

### What is Markdown?
Markdown is a lightweight markup language used to add formatting to plaintext. It's used in Hugo to write content, which Hugo then renders into HTML.

### How do I add a post?
To add a post, use `hugo new posts/[post-name].md`. This command creates a Markdown file where you can write your post.

## Themes and Appearance

### What is a Hugo theme?
A theme dictates the appearance of your site and includes templates, content types, and resources to style your site. Themes can be found on [Hugo Themes](https://themes.gohugo.io/) or you can create your own.

## Advanced Features

### Multilingual Support and Output Formats
Hugo supports multiple languages and can output content in formats like HTML, JSON, RSS, and CSV.

### Shortcodes and Custom Content
Shortcodes allow you to insert complex HTML snippets or custom content that doesn't fit regular Markdown syntax.

## Development and Deployment

### How do I handle static assets?
Place static assets like images and JavaScript in the `static` folder. Hugo will copy these into the `public` directory at build time.

### How can I preview my site locally?
Run `hugo server` to start a local web server. Your site will be available at `http://localhost:1313/`.

### How do I deploy my Hugo site?
After building your site with the `hugo` command, upload the `public` directory to your hosting service or use CI/CD platforms like Netlify, Vercel, or GitHub Pages for deployment.

## Updates and Troubleshooting

### How do I update Hugo?
- **macOS:** Use `brew upgrade hugo`
- **Windows:** Use `choco upgrade hugo`
- Alternatively, download the latest version from the [Hugo GitHub](https://github.com/gohugoio/hugo) page.

## Example of Hugo Code Usage

```html
{{ '<html><head><title>{{ .Site.Title }}</title></head><body>' | safeHTML }}
<h1>{{ .Title }}</h1>
{{ .Content }}
</body></html>
```
This template example shows how to use Hugo's templating to include the site title, page title, and content.

For more detailed information on using Hugo, refer to the [Hugo Documentation](https://gohugo.io/documentation/).

This structured layout provides a cleaner, more navigable document. It separates broad topics into clear sections and uses questions as headings for quick scanning. The example code snippet is also neatly integrated to provide practical insight directly within the FAQ context.
