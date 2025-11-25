*Previously called "Spidertyler2005"*

# About me

I have been programming in python for over 9 years just working on hobby projects.

Recently I've started a position at Trevity LLC as a fullstack developer on an R&D team.


# Projects

### Currently working on my own compiled programming language named BCL.

If you are interested, star my project on github.

### Simple Serialize-to-Image

Take python data and represent it in the bytes of a 3-channel image file (rgb).
It also works the other way around. Very simple ~200 line module to be included in whatever
project you may way.

It was really a quick project I made while I was bored, but it has documentation
in the readme.md

### Nexonauts (developer) (Canceled)

Nexonauts in a space exploration game currently in development.

I am a developer working on this indie title and try to bring it to life with the help of the Lead Developer Nikk F.

You can wishlist the game on steam if you are interested!

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
