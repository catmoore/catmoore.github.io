
Instructions
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
2. Fork this repository by clicking the "fork" button in the top right.
3. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
4. Set site-wide configuration and create content & metadata (see below -- also see this set of diffs showing what files were changed to set up an example site for a user with the username "getorg-testacct")
5. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.
6. Check status by going to the repository settings, in the "GitHub pages" section
(Optional) Use the Jupyter notebooks or python scripts in the markdown_generator folder to generate markdown files for publications and talks from a TSV file.
See more info at https://academicpages.github.io/

To run locally (not on GitHub Pages, to serve on your own computer)
1. Clone the repository and made updates as detailed above
2. Make sure you have ruby-dev, bundler, and nodejs installed: sudo apt install ruby-dev ruby-bundler nodejs
3. Run bundle clean to clean up the directory (no need to run --force)
4. Run bundle install to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
5. Run bundle exec jekyll serve to generate the HTML and serve it from localhost:4000
6. Changelog -- bugfixes and enhancements
7. There is one logistical issue with a ready-to-fork template theme like academic pages that makes it a little tricky to get bug fixes and updates to the core theme. If you fork this repository, customize it, then pull again, you'll probably get merge conflicts. If you want to save your various .yml configuration files and markdown files, you can delete the repository and fork it again. Or you can manually patch.

To support this, all changes to the underlying code appear as a closed issue with the tag 'code change' -- get the list here. Each issue thread includes a comment linking to the single commit or a diff across multiple commits, so those with forked repositories can easily identify what they need to patch.
