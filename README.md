# My Learning Blog

A blog built with [Jupyter Book](https://jupyterbook.org/) to document what I learn. This blog is automatically deployed to GitHub Pages using GitHub Actions.

## 🚀 Features

- **Jupyter Book**: Create beautiful, publication-quality content
- **Automatic Deployment**: GitHub Actions automatically builds and deploys on every push
- **Markdown & Notebooks**: Write content in Markdown or Jupyter notebooks
- **GitHub Pages**: Free hosting directly from this repository

## 📖 How to Use

### Adding New Blog Posts

1. Create a new Markdown file (`.md`) or Jupyter notebook (`.ipynb`) in the `posts/` directory
2. Add your content using Markdown or notebook cells
3. Update `_toc.yml` to include your new post in the table of contents
4. Commit and push your changes - GitHub Actions will automatically build and deploy!

Example entry in `_toc.yml`:
```yaml
chapters:
  - file: posts/welcome
  - file: posts/first-blog-post
  - file: posts/your-new-post  # Add your new post here
```

### Local Development

To build and preview the blog locally:

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Build the book:
```bash
jupyter-book build .
```

3. Open the generated HTML in your browser:
```bash
# The output will be in _build/html/index.html
```

### Configuration

- `_config.yml`: Configure book settings, author, title, repository links, etc.
- `_toc.yml`: Define the structure and order of your content
- `requirements.txt`: Python dependencies for building the book

## 🎨 Customization

You can customize your blog by editing `_config.yml`:
- Change the title and author
- Modify the theme settings
- Add or remove features like comments, repository buttons, etc.

## 📝 Writing Tips

- Use Markdown for text-heavy posts
- Use Jupyter notebooks when you want to include executable code and visualizations
- Add images by placing them in an `images/` folder and referencing them in your content
- Use MyST Markdown extensions for advanced features like admonitions, tabs, and more

## 🔧 GitHub Actions Workflow

The deployment workflow (`.github/workflows/deploy.yml`) automatically:
1. Checks out your code
2. Sets up Python
3. Installs dependencies
4. Builds the Jupyter Book
5. Deploys to GitHub Pages

**Important**: Make sure GitHub Pages is enabled in your repository settings and set to deploy from GitHub Actions.

## 📚 Resources

- [Jupyter Book Documentation](https://jupyterbook.org/)
- [MyST Markdown Guide](https://myst-parser.readthedocs.io/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)

## 🤝 Contributing

Feel free to open issues or submit pull requests if you find any problems or have suggestions!