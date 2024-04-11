### Original Guide URL: 
```
https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/
```

### Alternatively:

1. Fork [this repository](https://github.com/therajmaurya/therajmaurya.github.io/fork): 
```
https://github.com/therajmaurya/therajmaurya.github.io/fork
```

2. Setup "ruby" using following version manager tool for the Ruby ("gem" will install automatically with ruby):
```
https://github.com/rbenv/rbenv
```

3. Next run the command on terminal to install bundler:

```bash
gem install bundler
```

4. Change directory to the cloned repo and run below command on terminal:

```bash
bundle
```

### File to be modified in the cloned Repo:

1. `_config.yml`: 
- This file is used to setup project level information for the entire site like personal details, page settings, google analytics tracking, etc.
- If you are testing changes locally, for any changes to this file, you need to restart the server to reflect the changes.
- This file would need to be changed mostly at the beginning of the project only. Incremental chaanges might be needed rarely if you want to add/enable any other feature or modify some existing behaviour.

2. `_data/navigation.yml`: 
- This file is used to setup the navigation options at the top of the website and link them to the _pages markdown files. 
- This file would need to be changed mostly at the beginning of the project only. Incremental chaanges might be needed rarely if you want to add/enable any other feature or modify some existing behaviour.

3. `_pages`:
- This folder contains the pages mentioned in "navigation.yml"
- "url" in the navigation file must match "permalink" in the corresponding markdown file in _pages folder. Filename of the markdown file could be anything, but to avoid confusion, keep markdown file name same as url and permalink.
- There are many more keys that you can set in additon to "permalink" in the beginning of the markdown files. You can explore different pages for the same other you may browse internet to explore more.
- Markdowns under this folder require lesser modficiation once the setup is done. Incremental chaanges might be needed only when you want to add/modify any other page/section.

4. `_posts`:
- This folder contains the markdowns of individual posts that you want to publish on the website. 
- Posts are named according to the YEAR-MONTH-DAY-title.MARKUP format. [Further Details: https://mmistakes.github.io/minimal-mistakes/docs/posts/]
- Similar to pages, eaach markdown in this folder also has some configurations at the beginning of the markdown like setting tags, category, title, excerpt, table of content, modified timestamp, etc. 
- Markdowns under this folder mostly would require changes as and when you add new posts.

5. `_includes/footer.html`:
- This file needs to be changed if you want to update the footer details.

### Note: 
- You will need to create folder at root - by post category and sub-folder by post title - to store artifacts for posts, if you want to attach any files to a post.
- You will also need to create folder at root - by page - to store aertifacts for pages, if you want to attach any files to a page.
- Markdown files support raw HTML script. Ex: I have used HMTL embed tag to render PDF on my site.
