# About me

Hi! I'm a self-taught programmer of over 10 years experience. My philosophy for software is that we should be kind to our own (other programmers) as well as the people we build software for.
We should work in cooperative structures when creating private businesses. Its important that we all look after each other and ensure that we all benefit from our own labor. As for customers/consumers- I think exploitative practices in modern software are ridiculous. Exploitation is commonplace. SaaS, online-only software, patenting of basic UI, and more- these are things that are employed when they shouldn't be. Sure- SaaS makes sense sometimes, but a simple application shouldn't cost an on-going fee and require internet connection to work.

Even developers making self-published software decide to be so unbelievably greedy at times. They can get away with it because its common practice. Its disgusting, abhorrent behavior and I do not respect those who willingly exploit others in such a way. 

The advent of browser based software/services has only made this worse. You can "reasonably" charge a monthly fee when all you provide is hosting. You, of course, almost always have the choice to make your software work without being in the browser. It also leads to mass data collection concerns when we centralize everything. Users have NO CHOICE in whether or not to have some data collected. Usage data inherently has to be collected for applications to work. For instance if you create a post on a website, that has to be logged. Change you settings? That too is written down somewhere. Liked a post? Also written down. Although this collection is an unintentional side-effect, it still can create a footprint that a user has no choice over. For some applications, this is unavoidable, for others- developers and business owners have simply made a choice to prevent you from owning your data.

We need let people own their data again. We need to let people OWN their software again. We need to let people MODIFY their own software copies.

# Job
I work at Trevity LLC as a fullstack developer on an R&D team.

# Donations
Feel free to donate to my [Patreon](https://www.patreon.com/c/ArachnidAbby). This will allow me to spend more of my time on these projects. If I get enough funding, I might even make this my job.... altho I doubt that would happen.


# Projects
## Summersweet-software/ComprehensiveConfig
A configuration validation/writer library that is extremely ergonomic and pythonic. It also has absolutely fantastic static typing that makes working with it a joy.

## Summersweet-software/CompilerToolkit
A library to help create compilers in python. It is an opinionated library that helps you enforce certain coding practices throughout your entire codebase. It is also well-typed which is something that isn't always true when writing a compiler by hand. This lets you actually focus on the static-type checking errors instead of ignoring them because you have a few hundred (or thousand)

## Summersweet-software/OpenPluginApi
A library to help you load and package plugins. It creates a standard way to load plugins and lays out a standard format for plugins. This library does plugin sorting, loading, packaging, and internal dependency management (allowing plugins to have their own dependencies or version of dependencies). It also does minimal isolation of plugins being loaded from the general project.

This was built for a product being privately worked on inside of Summersweet-software, but the component seems generally useful to anyone interested in plugin systems. It made sense to build a general purpose component.

## ComprehensiveTui
A library for creating TUI applications in a way similar to QT. It uses widgets and layouts. It includes a few base widgets that are very well made.
It also solves the problem of flickering in your TUI's main window or in its cursor.

## stoat-CLIent
A custom TUI client for stoat that I'm making for fun. Its the inspiration behind making a TUI library.

### Currently working on my own compiled programming language named BCL.

If you are interested, star my project on github.

### Simple Serialize-to-Image

Take python data and represent it in the bytes of a 3-channel image file (rgb).
It also works the other way around. Very simple ~200 line module to be included in whatever
project you may way.

It was really a quick project I made while I was bored, but it has documentation
in the readme.md

### Effects In Python

A very simple effects system made in python. Surprisingly usable despite just being a proof of concept.

```python
@EffectFunction
def yield_value(value):
    pass


YieldEffect = Effect(yield_value)


@UsingEffect(YieldEffect)
def traverse(data: list):
    match data:
        case [x, *data]:
            yield_value(x)
            traverse(data)
        case []:
            return


@ImplementEffect(YieldEffect, yield_value=lambda x: print(f"yielded {x}"))
def main():
    traverse([1, 2, 3])


main()
```
