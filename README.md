##Boy, with Jeet

A lightweight, up-to-date, version of HTML5 Boilerplate with conditionally loaded polyfills for amazing CSS3 support back to IE7.

Using the Jeet Grid System. Dope, right?

[Boy](https://github.com/corysimmons/boy)

[Jeet](https://github.com/mojotech/jeet)

Slapped together and modified by Tyler Steimle of Kmotion Design, in Grand Rapids, MI.



###Structure &amp; Elsewhere

In the spirit of the Jeet grid system&mdash;which is awesome because it keeps your grid in your stylesheets instead of your HTML&mdash;I've set up a basic modular structure for the default Sass files according to how I like to work on a project.

This project uses Compass. Hence, the config.rb file.

I've used [gitignore.io](http://www.gitignore.io) to generate my own gitignore file based on OS X, Sublime Text, Sass, and Codekit. You may want to generate your own.

In the `scss/base/_functions.scss` file I've basically ripped off Zurb's Foundation 5 rem-calc function and created an optional mixin in `scss/base/_typography.scss` that outputs a px fallback for older browser support. It looks like this in your wild:

    h1 {
      @include rem(40);
    }

And outputs this CSS:

    h1 {
      font-size: 40px;
      font-size: 2.5rem;
    }