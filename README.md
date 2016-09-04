# dst4l
Website for DST4L - Data Scientist Training for Librarians.
denne web er lavet med Jekyll, GitHub pages, bootstrap templates ....


## Guide to using and maintaining this website

### Simple usage

Adding or changing a simple file can be done directly via Github.


### Edit and preview localy on your own PC

#### Install Jekyll

See [Installing Jekyll on Windows](http://jekyll.tips/jekyll-casts/install-jekyll-on-windows/)


#### Fork and Clone the github repo.


#### Run Jekyll locally to preview changes

    jekyll serve --watch

#### Commit and make a pull-request


### Page types

#### Regular pages

HTML and Markdown pages can be added to the root of the repository. They will automatically be added to the menu.
All pages should start with metadata in Jekyll YAML format:

    ---
    title: Example Page
    ---

    This is an example page

#### Speaker pages

Each speaker should have a page in the `_speakers` directory. A speaker page should start with ta set of speaker specific metadata:

    ---
    speaker-id: johndoe
    fullname: John Doe
    shortname: John 
    image: speaker.gif
    affiliation: NSA
    twitter: johndoe
    email: "johndoe@nsa.gov"
    github: johndoe
    lead: "John is a leader in annonymity on the net, and IRL"
    role: Placeholder
    ---

    A longer description of the speaker goes here...

Hopefully most of the metadata is self explanatory. The `speaker-id`should be unique, and is used as reference from events (presenetations/workshops)

















### Reference

[Kramdown](http://kramdown.gettalong.org/syntax.html) is the *MarkDown* flavour that is being used to write simple text pages. (The files the the extension: `.md`)

[Jekyll](https://jekyllrb.com) is used to process the markdown and partial html pages into a complete website.

[Github Pages](https://pages.github.com) is used to host the website. 
Github knows about jekyll, so github will use jekyll to create the website everytime new commits are pushed to github.

[Universal bootstrap theme](http://universal.ondrejsvestka.cz/1-0/index2.html) is used for stylesheets and layout.
It is free and has been downloaded from [bootstrapious](http://bootstrapious.com/p/universal-business-e-commerce-template).
It should be relatively easy to copy-paste any layout component you see in the theme into the DST4L website. 
If you need this simply write your page in HTML (use `.html` as extension)


[Bootstrap](http://getbootstrap.com) is used by the Universal theme to do the layout. 
So if you have special layout requirements you may need to check the boottrap documentation. 
Also, any 
[CSS](http://getbootstrap.com/css/) and
[Component](http://getbootstrap.com/components/)
from Bootstrap should be easy to use in the DST4L website.


