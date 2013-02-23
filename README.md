LiveReloadX
===========

![Edit & Reload](http://nitoyon.github.com/livereloadx/images/title.png)

User documentation is under http://nitoyon.github.com/livereloadx/.

This is developper documentation. 


Setting up a development environment
------------------------------------

First, clone a git repo by running:

```
git clone git://github.com/nitoyon/livereloadx.git
cd livereloadx
```

Install dependant modules:

```
npm install
```

Check out `gh-pages` branch if you wish to edit project page:

```
git new-workdir . gh-pages gh-pages
```

(ref) [git-new-workdir](https://github.com/git/git/blob/master/contrib/workdir/git-new-workdir), [git-new-workdir-win](https://github.com/dansmith65/git/blob/master/contrib/workdir/git-new-workdir-win)



Running tests
-------------

Run mocha.

```
./node_modules/.bin/mocha
```


Edit project page
-----------------

Install Ruby and Jekyll:

```
gem install jekyll
```

Run Jekyll on `gh-pages` branch:

```
jekyll --auto
```

Run LiveReloadX:

```
livereloadx -s
```

Now open `http://localhost:35927/_site/` on your browser.


Related Projects
----------------

* [livereload](https://github.com/livereload/): Official version.
* [mklabs/tiny-lr](https://github.com/mklabs/tiny-lr): Tiny reimplementation of LiveReload 2.X server in node.js.
* [gruntjs/grunt-contrib-livereload](https://github.com/gruntjs/grunt-contrib-livereload): Grunt task.
* [josh/node-livereload](https://github.com/josh/node-livereload), [clonn/simple-livereload](https://github.com/clonn/simple-livereload), [khoomeister/livereloaded](https://github.com/khoomeister/livereloaded): Reimplementation of LiveReload 1.X server in node.js
* [usualoma/node-livereload-hub](https://github.com/usualoma/node-livereload-hub): Yet another reimplementation of LiveReload 1.X server (Reload via the HTTP request)
* [guard/guard-livereload](https://github.com/guard/guard-livereload): Ruby implementation running with guard.

