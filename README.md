> [!WARNING]
> Tincta is no longer available in the App Store as it is not working reliably on macOS Ventura and later.


# Tincta

Free text editor for Mac with focus on speed, stability and ease of use.

![Tincta screenshot](/website-images/Screenshot.png?raw=true)

## Features

**Tincta comes with all the features you expect from a professional text editor:**

- Syntax coloring for over 65 languages
- Search and replace with RegEx support
- Fast and reliable line numbering
- Full unicode support
- Multiple built in color themes
- Custom color themes
- Fast and snappy native Mac app

**And lots of useful little details that will make you love it:**

- Auto close brackets
- Auto indent lines
- Page guide
- Automatically wrap lines
- Full drag & drop support
- Indent selected text with tab
- Search and replace with RegEx support
- Change case
- Show invisible characters
- Convert between text encodings
- Convert line endings
- Convert tabs/spaces
- Spell checker
- Printing
- Block selection
- Octopus icon


## Official website and more product info

[Here it is](https://codingfriends.github.io/Tincta/)


## Status

We started Tincta in 2011 (!). Already on macOS Monterey, we noticed an increase of app crashes. In the Ventura, Tincta sometimes would not even launch anymore. We could never really locate nor fix these crashes. Tincta’s codebase is over 10 years old and was originally built for MacOS Snow Leopard. Since then, macOS has moved on not only from cats to landmarks but also technically. But Tincta, being a free app and one of our side projects, could not keep up.

For a while now we concentrate our efforts on
[Wokabulary — The best flash card learning app for Mac and iPhone](https://wokabulary.com).

We keep Tincta’s source on GitHub as a reference and for anybody who wants to build it themselves.



## Build

It should just compile with XCode. There are two caveats, though:

* We have our dev certificate setup in the project so you need to remove that or replace it with your own
* The App Store build includes the Sentry crash reporter. The private key is defined in the `SentryConfig.h` which is not included in the source. There is a `SentryConfig_Example.h` that you can use for your own Sentry account. Or you can delete all references to it alltogether and remove the import from `Tincta-AppStore-Prefix.pch`
