# Gemini [![Build Status](https://travis-ci.com/lyuwen/gemini.svg?branch=master)](https://travis-ci.com/lyuwen/gemini)

Gemini is a modern LaTeX [beamerposter] theme.
This is a modified version that does not require LuaLaTeX,
  the original version is [**here**](https://github.com/anishathalye/gemini).


## Dependencies

* A TeX installation.
* LaTeX package dependencies including beamerposter (these usually come with
  your TeX installation, but if not, you can get them from [CTAN])

## Usage

1. Copy the files in this repository (or clone the repository)

1. In `poster.tex`, set up your paper size, column layout, and scale the
   content as necessary

1. Make a copy of `beamercolorthemegemini.sty`, update the `\usecolortheme`
   line in `poster.tex`, and theme the poster to your liking (optional, but
   highly recommended)

1. Run `make` to build your poster

## Themes

Gemini currently includes three color themes:

* `default`
* `gemini`
* `mit`
* `labsix`

## Custom define color schemes

With `gemini` color theme, user now have the freedom the custom define their color schemes.
To define a custom scheme, put set following color names to the desired colors before the command
`\usecolortheme{gemini}`:

```
\definecolor{accentcolor}{RGB}{62, 138, 189}
\definecolor{textcolor}{0, 0, 0}
\definecolor{bgcolor}{RGB}{255, 255, 255}
```

Additionally the following colors will by default be a mixture of the three colors defined above,
but it is also possible to override those preset mixing rules:

```
\definecolor{lighttextcolor}{RGB}{215, 217, 218}
\definecolor{darkbgcolor}{RGB}{19, 76, 113}
```

Alternative to `\definecolor` command, `\colorlet` command can also be used to define color using
those already defined colors, either simply aliasing or a mixing of some colors.

The alternative themes are intended to be inspiration for you to make your own
color theme. You're highly recommended to make your own color theme (it's
really easy!) or use the default Gemini theme.

### Gemini theme

<p align="center">
<a href="https://raw.githubusercontent.com/lyuwen/gemini/assets/poster-gemini.pdf">
<img src="https://raw.githubusercontent.com/lyuwen/gemini/assets/poster-gemini-small.png">
</a>
</p>

### MIT theme

<p align="center">
<a href="https://raw.githubusercontent.com/lyuwen/gemini/assets/poster-mit.pdf">
<img src="https://raw.githubusercontent.com/lyuwen/gemini/assets/poster-mit-small.png">
</a>
</p>

### LabSix theme

<p align="center">
<a href="https://raw.githubusercontent.com/lyuwen/gemini/assets/poster-labsix.pdf">
<img src="https://raw.githubusercontent.com/lyuwen/gemini/assets/poster-labsix-small.png">
</a>
</p>

## Design goals

* **Minimal**: clean and easy to read, so that the emphasis is on the content
* **Batteries included**: works and looks good out of the box
* **Easy theming**: easy to create and use a new color theme

## Contributing

Contributions to Gemini such as bug reports, new themes, and new poster
components are greatly appreciated! Given the subjective nature of design,
you're encouraged to open an issue or pull request early to get feedback before
investing a lot of time in implementing a new feature.

## License

Copyright (c) 2018-2019 Anish Athalye. Released under the MIT License. See
[LICENSE.md][license] for details.

Copyright (c) 2020 Lyuwen Fu.

[beamerposter]: https://github.com/deselaers/latex-beamerposter
[CTAN]: https://ctan.org/
[license]: LICENSE.md
