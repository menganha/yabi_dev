date: 2022-12-12
draft: no

# Getting started with yabi

Once yabi is installed, say, you want to create a new blog that describes your
philosophical thoughts. You call it *Discourses*. To create this new blog type
in a terminal

    yabi init Discourses

now navigate to the newly created folder

    cd Discourses

To publish your first though, create a new file on, e.g.,
`posts/my_first_thought.md`. The only requirements for a post is that

1. It is somewhere inside the `posts` folder
2. Has set the label `draft` to "yes" or "no" at the file header.
3. It has a level 1 Markdown heading with the title of the post right after the label(s).

Apart from these minimal requirements, the post can have any valid Markdown syntax.

    draft: no
    
    # My first thought

    I will drink more water. I will exercise more and I will wake up earlier.

    No, I'm not. I rather not to.

Finally, build the website using the command

    yabi build

All the contents of the website are built under the folder `public`. You can
upload these files to any hosting service of your liking. If you wish to check
how the site will look you can use the command

    yabi test

which will create a local server with your website on `http://localhost:9090` by
default.
