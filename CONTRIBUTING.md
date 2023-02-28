# Contributing guide

## Prerequisites

No prerequisites exist.

## How to get started?

Before writting your own page try explore existing ones.
Start with [one](./common/sleep.clip) of the simplest pages.

Each page should explain the following aspects of described commands:

- command properties like it's name, way to get full documentation
- command examples, at least one

To make user see where it's allowed to write some arbitrary (but valid) content
it's allowed to surround some piece of text with curly braces like
`{int character count}`.

Given already mentioned page above:

```md
# sleep

> Delay for a specified amount of time
> Help: --help
> Version: --version
> More information: https://www.gnu.org/software/coreutils/sleep

- Delay in seconds:

`sleep {int seconds}`

- Delay in [m]inutes:

`sleep {int minutes}m`

- Delay in [h]ours:

`sleep {int hours}h`
```

Here we can see that the first line is a page header. All lines starting with an
opening angle bracket explain common command properties like what it does (at
first), how to get help, version and full documentation. Code examples are written
down below. Their explanations start with one single dash, while code itself is
surrounded with backticks.
