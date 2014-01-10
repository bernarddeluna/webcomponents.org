# Web Components Strawman

Home to the Web Components strawman site. This is where pioneers and community-members of the Web 
Components ecosystem (like Polymer, X-tags, and other interested parties) document web components 
best practices so that others can follow the same path instead of needlessly striking out on their own.

We welcome any and all contributions. Please feel free to get involved on the issue tracker.

## Why WebComponents.org?

One of the driving goals behind WC.org is that long-term some of our goals include features which are not strictly documentation on the platform:

* Best practices around component authorship when it comes to polyfills and frameworks built on top of web components. Imo, docs for platform features (Shadow DOM, Imports etc) eventually should go on WPD but best practices are something subjective that the community should be able to evolve in the open. I see this type of content being a better fit for WC.org.
* Enabling a search and discovery mechanism for Web Components authored by the community (search + gallery + voting to surface high-quality components) built on top of existing package management solutions
* Enabling a central point of discussion around WCs (once again that are vendor-neutral). 

The audience is less novice developer and more advanced developer. It's a place where vendors and savvy developers can chat.

## Getting started

The site is made with [Jekyll](https://github.com/mojombo/jekyll/), a static generator in Ruby. It also uses [redcarpet](https://github.com/vmg/redcarpet) to process the markdown in the site.

The best way to install Jekyll and Redcarpet is via RubyGems:

```
gem install jekyll redcarpet
```

Once Jekyll is installed, you just need to clone the project:

```
git clone --recursive git@github.com:WebComponentsOrg/webcomponents.org.git
```

Then go to the project's folder:

```
cd webcomponents.org
```

If you are using Git 1.6.4 or earlier, you will manually need to initialize the submodules:

```
git submodule update --init
```

You should now have a copy of the source files for the site that are ready for editing.

## Jekyll commands

Jekyll has three basic options used in this project:

To generate the site and run it in a server, which can be viewed at `http://localhost:4000`, run:

```
jekyll server
```

To regenerate the site as you edit and save files, run:

```
jekyll server --watch
```

To generate a static version of the site that is ready to upload to a server (it will create a folder called _site), run:

```
jekyll build
```

## License

Source code is available under [MIT](http://opensource.org/licenses/MIT) license and content is under [Creative Commons BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/deed.en_US).
