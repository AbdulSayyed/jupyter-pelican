# nipype folder

- This is a main `nipype` folder and `nipype` conda environment.
- I am going to install `jupyter-pelican` here to see how my static blogs works.

# Installing pelcan using help from [here](https://pythonforundergradengineers.com/how-i-built-this-site-1.html).

 1. pip install markdown
 2. pip install pelican
 3. pip install fabric3
 4. pip install bs4
 5. pip install ghp-import

  > I get this error - >ERROR: nbconvert 5.6.1 requires entrypoints>=0.2.2, which is not installed.

  ## Creating a remote repo name `jupyter-pelican`

  1. Created and pulled it locally.
  2. pelican-quickstart.

```txt
   Where do you want to create your new web site? [.] 
> What will be the title of this web site? nipype
> Who will be the author of this web site? Abdul Sayyed
> What will be the default language of this web site? [en] 
> Do you want to specify a URL prefix? e.g., https://example.com   (Y/n) Y
> What is your URL prefix? (see above example; no trailing slash) http://AbdulSayyed.github.io/jupyter-pelican
> Do you want to enable article pagination? (Y/n) y
> How many articles per page do you want? [10] 5
> What is your time zone? [Europe/Paris] Europe/London
> Do you want to generate a tasks.py/Makefile to automate generation and publishing? (Y/n) y
> Do you want to upload your website using FTP? (y/N) n
> Do you want to upload your website using SSH? (y/N) n
> Do you want to upload your website using Dropbox? (y/N) n
> Do you want to upload your website using S3? (y/N) n
> Do you want to upload your website using Rackspace Cloud Files? (y/N) n
> Do you want to upload your website using GitHub Pages? (y/N) y
> Is this your personal page (username.github.io)? (y/N) y
Done. Your new project is available at /home/sayyed/neuro-science/projects/nipype


```

 ## Serving the document

 1. make serve
 2. Check your `localhost:8000`
 3. The directory structure is show below.

 ```txt
 rwxrwxr-x 2 sayyed sayyed 4.0K Jul  5 03:09 content/
drwxrwxr-x 6 sayyed sayyed 4.0K Jul  3 22:35 Ex-01/
-rw-rw-r-- 1 sayyed sayyed 2.9K Jul  5 03:09 Makefile
drwxrwxr-x 3 sayyed sayyed 4.0K Jul  5 03:10 output/
-rw-rw-r-- 1 sayyed sayyed  856 Jul  5 03:09 pelicanconf.py
-rw-rw-r-- 1 sayyed sayyed  633 Jul  5 03:09 publishconf.py
drwxrwxr-x 2 sayyed sayyed 4.0K Jul  5 03:10 __pycache__/
-rw-rw-r-- 1 sayyed sayyed 1.8K Jul  5 03:13 ReadMe.md
-rw-rw-r-- 1 sayyed sayyed 3.6K Jul  5 03:09 tasks.py
sayyed@neuro ~/n/p/nipype (master)>  
```

### Adding first post 

1. Created `nipype.md` in content folder
2. Added and committed then push to remote.

### Adding [themes](https://github.com/getpelican/pelican-themes)

1. Adding themes as a submodule in the main directory. `git submodule add https://github.com/getpelican/pelican-themes.git`. it is added from the main directory.
2. Initilize the submodule

```
git submodule add https://github.com/getpelican/pelican-themes.git
$ git submodule init
$ git submodule update --init --recursive
---
git submodule add https://github.com/getpelican/pelican-plugins.git
$ git submodule init
$ git submodule update --init --recursive

```

---
[//]:# (Note to self: I have to add changes to my jupy-pelican repot. This changes contain of adding themes and plug in directory but since they are huge I do not want to add them until I am sure that which them I am going to use. The rest will be deleted. Sam applies to submoudle.)

[ ] Tomorrow I ahave to start frm [here](/https://pythonforundergradengineers.com/how-i-built-this-site-3.html).
