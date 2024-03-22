
[Follow the instructions here in ottrproject.org](https://www.ottrproject.org/editing_website.html) for details on how to start editing your OTTR website.

The following files need to be edited to get this new website started!

### Files that need edited upon creating a new website.

- [ ] `README.md` - Fill in the README with the title of the website, a brief description of the website, and any other details that would be useful for anyone who encounters your website.
- [ ] `index.Rmd` - Update the `title` field. Since this Rmd file serves as the website's landing page, include any information you believe will be beneficial for visitors upon their arrival.


### Files that need to be edited upon adding each new page.

- [ ] `_site.yml` - Include the title of your newly created page in the `text` field, and insert the corresponding html file name into the `href` field.

### Picking a style

See more [about customizing style on this page in the guide](https://www.ottrproject.org/customize-style.html).
By default this website template will use the jhudsl data science lab style. However, you can customize and switch this to another style set.

#### Using a style set

[Read more about the style sets here](https://www.ottrproject.org/customize-style.html#Using_a_style_set).

- [ ] On a new branch, copy the `style-sets/<set-name>/index.Rmd` and `style-sets/<set-name>/_output.yml` to the top of the repository to overwrite the default `index.Rmd` and `_output.yml`.
- [ ] Copy over all the files in the `style-sets/<set-name>/copy-to-assets` to the `assets` folder in the top of the repository.
- [ ] [Create a pull request](https://www.ottrproject.org/writing_content.html#Open_a_pull_request) with these changes, and double check the rendered preview to make sure that the style is what you are looking for.

### Files that need to be edited upon adding new packages that the book's code uses:

- `docker/Dockerfile` needs to have the new package added so it will be installed. See [instructions](https://www.ottrproject.org/customize-docker.html).
- The code chunk in `index.Rmd` should be edited to add the new package.
