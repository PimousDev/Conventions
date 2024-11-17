![Pimous Dev. Banner](https://github.com/PimousDev/.github/blob/master/Content/Images/PimousDev_banner.jpg?raw=)
# Conventions [![License badge](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgray)](LICENSE.txt)
Pimous Dev. Conventions are universal conventions for computer developement that
every Pimous Dev. project should follows. However, there aren't meant to be
adopted by a wide range of developers, but to only be used internally to help us
understand and maintain our own projects. In this way, every poject will look,
be used and developed the same way. _However, if you still want to follow them,
go ahead! Maybe there're not that bad?_

This repository list all published and drafted conventions. They should follow
the template defined (See
[Contributing](#contributing)).

> Version: **-**

## Table of contents
_Soon..._

## Contributing
First of all, new pages should always be created on a new branch named
`<category>_<title>` under the path:
```
/conventions/<category>/<title>.md
```
where `category` refers to the category of the new page (In camel case) and
`title` to the unique title of the new page (Also in camel case).

Next, any commit to a page should always follows the format:
```
(<category>)[<title>] <commit>.
```
where parameters are the same than before, except for `commit` corresponding
to the title of the commit. Moreover, there is no restriction for description of
the commit.

Finally, to simplify writing of new pages, each ones should follows this
template [`template.md`](template.md).

### Description table
After the title of the template, there is a table giving information about the
convention written in the page:
- **`Status`:** Indicates current status of the page. Value should be either
`Not started`, `To write`, `To review`, `Under study`, `In writing`,
`In reviewing`, `Published`, `Deprecated` or `Canceled`.
- **`Verification`:** Indicates till when the page is still verified and
approved. Usually, it should last at least 4 months. Value should follow
`Until <date>` where `date` refer to the invalidating date represented in
[RFC 5322 (Section 3.3)](https://www.rfc-editor.org/rfc/rfc5322#section-3.3)
date format without `time`.
- **`Authors`**: Indicates authors and contributors of the page, usually as
links to their GitHub page.
- **`Create date`**: Indicates creation date of the page, represented in
[RFC 5322 (Section 3.3)](https://www.rfc-editor.org/rfc/rfc5322#section-3.3)
date format without `time`.

### Sections
After the description table, there is several sections partioning the page:
- **##Roadmap:** Lower than all other sections, it contains next tasks to do on
this page. Should always be removed when finished, before publishing.
- **#Convention:** Contains the convention of the page. The first paragraph
should be a good introduction summarizing the convention with links to useful
information for users.
- **#Links:** Contains links to other pages where their content is related to
this convention.
- **#References:** Contains an ordered list of the convention references, in
[IEEE reference format](https://journals.ieeeauthorcenter.ieee.org/wp-content/uploads/sites/7/IEEE_Reference_Guide.pdf).
You can use this tool to generate a reference: https://app.bibguru.com.

## License
<p xmlns:cc="http://creativecommons.org/ns#" xmlns:dct="http://purl.org/dc/terms/"><a property="dct:title" rel="cc:attributionURL" href="https://www.github.com/PimousDev/Conventions">Conventions</a> by <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://www.pimous.dev/">Pimous Dev.</a> are licensed under <a href="https://creativecommons.org/licenses/by-nc/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">CC BY-NC 4.0<img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt=""><img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1" alt=""></a> at <a href="LICENSE.txt">LICENSE.txt</a>.</p> 

## Authors
> Xibitol