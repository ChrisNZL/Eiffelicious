# Eiffelicious

### C# syntax theme for Atom 1.24.1

If you:

- Code in C#
- Fancy having method and property declarations stand out
- Are okay with using an older version of Atom
- Don't require Visual Studio for getting work done, and
- Don't mind wearing sunglasses

This theme might spice up your life.

Inspired from [TextMate](https://macromates.com/)'s [_Eiffel_ theme](https://inkdeep.github.io/TextMate-Themes/#eiffel), **_Eiffelicious_** works well with C# and [Atom 1.24.1](https://github.com/atom/atom/releases/tag/v1.24.1).

![Eiffelicious preview screenshot](https://i.imgur.com/dMO1wFo.png)

#### Why Atom 1.24.1?

Atom's ability to change font sizes for specific symbols is something unique compared to other editors.

Unfortunately, newer versions of Atom suffer from a regression of being incapable of detecting the difference between declarations and calls for methods and properties in C#, so all symbols of a method or property are affected by styling changes, regardless of context. 1.24.1 seems to be the last version that knows the difference.

Despite being an older version, Atom's generic multi-file intellisense autocompletion still works well without needing to rely on external code parsers.

#### Why _Atom_?

Atom's out-of-the-box search features just work, time and time again.

- <kbd>Ctrl</kbd>+<kbd>R</kbd>: Jump to any declaration in the current file.

- <kbd>Ctrl</kbd>+<kbd>T</kbd>: Jump to any file in any Project Folder you've added to Atom's sidebar.

- <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>F</kbd>: Search all files in your Project Folders for any text.

In a perfect world, everything would work without a hitch, but the lay of the land is:

- [Visual Studio](https://visualstudio.microsoft.com/vs/community/) is slow to launch, takes ages to update, is only for Windows (the macOS version is a different beast), and doesn't play nicely with Unity's project solutions. Too often, projects becomes unlinked, or Visual Studio's intellisense stops working after a DLL is changed, requiring you to reload all the files, and even then it doesn't always come back.

- [Visual Studio Code](https://code.visualstudio.com/) can't tell the difference between method and property declarations and calls for C#, and thus can't style them differently.

- [Sublime Text 3](https://www.sublimetext.com/3) does not detect C# property declarations when searching via <kbd>Ctrl</kbd>+<kbd>R</kbd>, and does not support generic multi-file intellisense.

- [OmniSharp](http://www.omnisharp.net/) doesn't always work.

- [Rider](https://www.jetbrains.com/rider/) is expensive.

As silly as it sounds, this particular version of Atom is my preferred C# editor, coupled with this theme.

#### Unity integration

If you develop games with [Unity](https://unity.com/), go Edit > Preferences > External Tools, and then:
1. For _External Script Editor_, browse for Atom.exe or Atom.app.
2. For _External Script Editor Args_, enter: `"$(File)":$(Line)`

![Unity preferences for Atom](https://i.imgur.com/b5Fto0F.png)

#### Issues and gotchas with Atom 1.24.1

- Before installing [Atom 1.24.1](https://github.com/atom/atom/releases/tag/v1.24.1):
  1. Disconnect your Internet connection so Atom doesn't update itself.
  2. Upon launch, go Help > About Atom, and uncheck _Automatically download updates_.


- Lines sometimes squish together. Restarting Atom sometimes helps, but you might need to pad your code with a couple blank newlines in places to make things readable.

- After closing a tab or file, Atom may stop suggesting autocomplete results and stop highlighting matching brackets. This can be resolved by reloading Atom via <kbd>Ctrl</kbd>+<kbd>Shift</kbd>+<kbd>F5</kbd>.

#### Recommended complementing packages
- [animated-page-scroll](https://atom.io/packages/animated-page-scroll)
- [atom-no-tab-close-icon](https://atom.io/packages/atom-no-tab-close-icon)
- [change-tabs](https://atom.io/packages/change-tabs)
- [color-tabs](https://atom.io/packages/color-tabs)
- [fancy-bracket-matcher](https://atom.io/packages/fancy-bracket-matcher)
- [minimap](https://atom.io/packages/minimap)
- [minimap-bookmarks](https://atom.io/packages/minimap-bookmarks)
- [multi-highlight-selected](https://atom.io/packages/multi-highlight-selected)
- [multiline-tab](https://atom.io/packages/multiline-tab)
- [open-files](https://atom.io/packages/open-files)
- [pinned-tabs](https://atom.io/packages/pinned-tabs)
- [smart-backspace](https://atom.io/packages/smart-backspace)
- [sublime-block-comment](https://atom.io/packages/sublime-block-comment)
- [symbols-tree-nav](https://atom.io/packages/symbols-tree-nav)
- [tab-title](https://atom.io/packages/tab-title)
- [title-bar-replacer](https://atom.io/packages/title-bar-replacer)
