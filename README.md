# About me

I have been programming in python for over 10 years just working on hobby projects.

I work at Trevity LLC as a fullstack developer on an R&D team.

# Donations
Feel free to donate to my [Patreon](https://www.patreon.com/c/ArachnidAbby). This will allow me to spend more of my time on these projects. If I get enough funding, I might even make this my job.... altho I doubt that would happen.


# Projects
## Summersweet-software/ComprehensiveConfig
A configuration validation/writer library that is extremely ergonomic and pythonic. It also has absolutely fantastic static typing that makes working with it a joy.

## Summersweet-software/CompilerToolkit
A library to help create compilers in python. It is an opinionated library that helps you enforce certain coding practices throughout your entire codebase. It is also well-typed which is something that isn't always true when writing a compiler by hand. This lets you actually focus on the static-type checking errors instead of ignoring them because you have a few hundred (or thousand)

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
