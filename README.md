# Project Description: Static Personal Blog with Python

#### Objective:
Create a static personal blog using Python to share your content and articles, with a simple design and clear navigation. This project is ideal for those who want a lightweight site that's easy to maintain and fast to load, as it doesn’t rely on a complex backend.

#### Tools and Technologies:
- **Python**: To generate the static content for the site.
- **Jinja2**: Template engine to render HTML pages dynamically but statically.
- **Markdown**: To write post content simply, converting it to HTML.
- **HTML/CSS**: For structuring and styling pages.
- **GitHub Pages / Netlify**: To host the static site for free. (Optional)

#### Project Structure:
1. **Project Setup**
   - Set up the directory structure to organize content and pages. Example:
     ```
     my_blog/
     ├── templates/
     │   └── base.html       # Base template for all pages
     ├── posts/
     │   └── sample_post.md  # Example post in markdown
     ├── output/
     │   └── index.html      # Rendered main page
     └── build.py            # Python script to generate the site
     ```

2. **Build Script (`build.py`)**
   - Create a Python script to:
     - Load HTML templates (Jinja2).
     - Convert Markdown files to HTML.
     - Organize posts by date and generate HTML for each post.
     - Generate a homepage with a list of recent posts.

3. **HTML Template with Jinja2**
   - Create a base template (`base.html`) with header, footer, and navigation links.
   - Create a specific template for posts and the homepage.

4. **Markdown to HTML Conversion**
   - Use Python’s `markdown` library to convert `.md` files to HTML.
   - Load the Markdown content into the HTML template for each post.

5. **Generating Static Pages**
   - The `build.py` script loops through all files in the `posts` folder, renders the corresponding HTML, and saves it in the `output` folder.
   - The homepage lists recent posts with links to each one.

6. **Deploy to GitHub Pages or Netlify (Optional)**
   - After generating the HTML files, deploy the site on a free hosting platform.
   - Set up GitHub Pages or Netlify to automatically update the site with new repository changes.
