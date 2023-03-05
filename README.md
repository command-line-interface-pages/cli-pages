# Command Line Interface (CLI) pages

Command Line Interface (CLI) pages.

## Current goals :checkered_flag:

- Update all coreutils pages to support all [v2.7.0 syntax](https://github.com/command-line-interface-pages/syntax/blob/main/base.md)
  features like availability of `--help`/`--version` options everywhere, switching
  between long/short options

## Quick introduction :rocket:

To get help for `cat` command type `clip-view cat`. If you need a more beautiful
output you can use [this](https://github.com/command-line-interface-pages/themes/tree/main/awesome)
theme like this: `clip-view --theme awesome cat`

![clip page](./clip-page.png)

Theme is a YAML file itself.

## Writing pages :hammer_and_wrench:

Read [this](./CONTRIBUTING.md) guide for details.

## Similar projects :books:

> :bell: Default render settings and official clients are used.

- [TlDr](https://github.com/tldr-pages/tldr) project with similar goal but with
  much less expressive syntax. Here is a `cat` page in TlDr:

  ![tldr page](./tldr-page.png)

- [Cheat](https://github.com/cheat/cheat) cheat allows you to create and view
  interactive cheatsheets on the command-line. Here is a `cat` page in Cheat:

  ![cheat page](./cheat-page.png)

## Why to use this project :question:

From page writer perspective:

- Write less, gain more:
  - Just mention how to get help or version of some command and get automatically
    generated code examples for these options.
  - Just mention that command is not intended for a direct usage or is deprecated
    and get automatically generated note about it.
- Write using unambiguous syntax:
  - Define when some command and when uses some I/O stream and be sure that
    code explanations have just one possible interpretation.
  - Define strict placeholder interpretation and type. Don't guess what some file
    with some extension is in example, know it's meaning directly from code.
- Permit user to use their preferences:
  - Don't use the most appropriate option's style from your opinion. Let user chose
    what option's style is the best for them while switching between GNU-style
    long and short options.
- Write in parsable format:
  - Be able to automatically extract information from pages and be sure about it's
    semantic.

From the end user perspective:

- Know how to get software builtin help or version.
- Be aware when and what commands to use and what not.
- Know when command uses and what I/O stream.
- Don't google what some not familiar file is, see it's description right here.
- Be yourself, and not the other person. Chose your code option's style.
