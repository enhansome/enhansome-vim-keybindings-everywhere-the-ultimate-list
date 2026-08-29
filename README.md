# Awesome Vim Keybindings Everywhere - The Ultimate List with stars

[![\<magic-marker-nbr-native>](https://img.shields.io/badge/Native%20programs%20listed-186-brightgreen)](#)
[![\<magic-marker-nbr-extensions>](https://img.shields.io/badge/Extensions%20listed-79-blue)](#)
[![Closed issues](https://img.shields.io/github/issues-closed/erikw/vim-keybindings-everywhere-the-ultimate-list?color=success)](https://github.com/erikw/vim-keybindings-everywhere-the-ultimate-list/issues?q=is%3Aissue+is%3Aclosed) ⭐ 2,583 | 🐛 0 | 🌐 Shell | 📅 2026-08-17
[![Closed PRs](https://img.shields.io/github/issues-pr-closed/erikw/vim-keybindings-everywhere-the-ultimate-list?color=success)](https://github.com/erikw/vim-keybindings-everywhere-the-ultimate-list/pulls?q=is%3Apr+is%3Aclosed) ⭐ 2,583 | 🐛 0 | 🌐 Shell | 📅 2026-08-17
[![OSS Lifecycle](https://img.shields.io/osslifecycle/erikw/vim-keybindings-everywhere-the-ultimate-list)](https://github.com/Netflix/osstracker) ⭐ 380 | 🐛 18 | 🌐 Scala | 📅 2024-03-10
[![License](https://img.shields.io/github/license/erikw/vim-keybindings-everywhere-the-ultimate-list?color=lightgrey)](LICENSE.txt)
[![Bump count of tools listed](https://github.com/erikw/vim-keybindings-everywhere-the-ultimate-list/actions/workflows/bump_tool_count.yml/badge.svg)](https://github.com/erikw/vim-keybindings-everywhere-the-ultimate-list/actions/workflows/bump_tool_count.yml) ⭐ 2,583 | 🐛 0 | 🌐 Shell | 📅 2026-08-17

[![Contributors](https://img.shields.io/github/contributors/erikw/vim-keybindings-everywhere-the-ultimate-list)](https://github.com/erikw/vim-keybindings-everywhere-the-ultimate-list/graphs/contributors) ⭐ 2,583 | 🐛 0 | 🌐 Shell | 📅 2026-08-17 including these top contributors:<br> <a href = "https://github.com/erikw/vim-keybindings-everywhere-the-ultimate-list/graphs/contributors"> <img src = "https://contrib.rocks/image?repo=erikw/vim-keybindings-everywhere-the-ultimate-list&max=36"/> </a>

> \[!NOTE]
> **:rocket: PRs are very welcome**

## What is this list?

Once your fingers have [learned](https://www.thejach.com/view/2012/07/vims_learning_curve_is_wrong) to speak Vim, they don't want to speak anything else! It's simply a very effective way of navigating, creating, and editing text. Thus, it's natural that one would like to get Vim-like keybindings in as many programs we use as possible.

The intention of this collaborative list is to:

* learn which programs/apps you already use, which you can enhance with Vim keybindings. Search in your browser with `ctrl/cmd + f`.
* discover new programs that support Vim keybindings. In need of a new file manager? Why not get one that has Vim keybindings?
* be up-to-date and alive -- add new programs and extensions as they evolve!

There are, of course, already lists like this one floating around on the internet (see [Acknowledgments](#acknowledgments)). While they are great, the issue is that they are not up-to-date with the latest developments. Vim-emulator add-ons are being developed all the time! This is why this collaborative list was created.

(yes, technically it is **vi**-like keybindings we talk about here, but most people know and Google for vim, thus vim is used here instead of vi).

> \[!TIP]
> **Tip**: navigate this document easily by using GitHub's built-in Markdown Table of Contents in the top right corner: <a href="#" title="GitHub built-in Table of Contents for markdown files."><img src="img/github_md_toc.png" width="256" alt="ToC"></a>

## Legend

The following symbols and formatting are used with each list item to make it clearer what kind of Vim keybindings support exist:

* :white\_check\_mark: - built-in support (possibly via a setting)
* :heavy\_plus\_sign: - via addon/extension
* ~~strikethrough~~: deprecated or unsupported software

Terminology:

* [TUI](https://itlaw.fandom.com/wiki/Text_user_interface) - Text User Interface

# The Ultimate Vim Keybinding List

## Debuggers

* :white\_check\_mark: [vimpdb](https://github.com/gotcha/vimpdb) ⭐ 206 | 🐛 7 | 🌐 Python | 📅 2017-02-19 - An integration of the Python debugger `pdb` and vim.
* :white\_check\_mark: [cgdb](http://cgdb.github.io/) - a curses interface on top of the GDB debugger with keybindings modeled after vim.

## Development

* :white\_check\_mark: [ptpython](https://github.com/prompt-toolkit/ptpython) ⭐ 5,450 | 🐛 265 | 🌐 Python | 📅 2025-11-21 - A better Python REPL. Start it with `ptpython --vi` or add `repl.vi_mode = True` to its `config.py`.

* :white\_check\_mark: [ipython](https://ipython.org/) - Interactive Python shell. It no longer uses readline for input, so it must be configured in the ipython profile `~/.ipython/profile_default/ipython_config.py` itself ([reference](https://gist.github.com/sstirlin/c3c207b1052b613ab9554b4ebdfc3f35)):

  * ```ini
    c.TerminalInteractiveShell.editing_mode = "vi"
    ```

* :white\_check\_mark: [GHCi](https://wiki.haskell.org/GHC/GHCi) - Interactive Haskell environment. It uses [haskeline](https://hackage.haskell.org/package/haskeline) instead of readline. Put this in `~/.haskeline`:

  * ```yaml
    editMode: Vi
    ```

* :heavy\_plus\_sign: [Jupyter Lab](https://pypi.org/project/jupyterlab-vim/) - Science and Data Development notebook environment. Add this package [jupyterlab-vim](https://pypi.org/project/jupyterlab-vim/) and restart the server. It is available for both `pip` and `conda` managed environments (and their derivatives).

* :white\_check\_mark: [marimo](https://marimo.io/) - An open-source reactive Python notebook that's stored as a .py file, executable as a script, and deployable as an app. Supports importing and exporting as Jupyter Notebooks. Built-in [vim keybinds](https://docs.marimo.io/guides/editor_features/overview/#vim-keybindings).

* :white\_check\_mark: [LINQPad](https://www.linqpad.net/) - The .NET Programmer’s Playground. vi mode is available in settings. To enable, go to Edit > Preferences > vi mode. Quite limited, doesn't support ex commands, registers, and macros.

* [Azure Data Studio](https://azure.microsoft.com/en-us/products/data-studio/) - Database tool similar to Microsoft SQL Server Management Studio. Supports VSCode extensions.
  * :heavy\_plus\_sign: [Vim plugin](https://github.com/VSCodeVim/Vim) ⭐ 15,201 | 🐛 1,906 | 🌐 TypeScript | 📅 2026-08-28 - Cannot be installed directly in the plugin section. Go to [Vim plugin release page](https://github.com/VSCodeVim/Vim/releases) ⭐ 15,201 | 🐛 1,906 | 🌐 TypeScript | 📅 2026-08-28 and download `.vsix` file. Inside Azure Data Studio, navigate to Extensions > three dots at the top > Install from VSXI. You will likely see the message: "Unable to install extension 'vscodevim.vim' as it is not compatible with the current VS Code engine version". If you see that message, you should try an earlier release.

* :white\_check\_mark: [Google Colab](https://colab.research.google.com/) - Data analysis and machine learning tool that allows you to combine executable Python code and rich text along with charts, images, HTML, LaTeX, and more into a single document stored in Google Drive. Vi modeis  supported through [keyboard binding settings](https://colab.research.google.com/notebooks/editor_details.ipynb#scrollTo=bEXkvERUtU5O). You can [enable](https://stackoverflow.com/questions/48674326/is-there-a-way-to-use-vim-keybindings-in-google-colaboratory) it through Tools > Settings > Editor

* [The Julia Programming Language](https://julialang.org/) - High-level, general-purpose dynamic programming language suited for numerical analysis and computational science
  * :heavy\_plus\_sign: [VimBindings.jl](https://github.com/caleb-allen/VimBindings.jl) ⭐ 123 | 🐛 28 | 🌐 Julia | 📅 2026-06-01 - A Julia package which emulates Vim directly in the Julia REPL

* :white\_check\_mark: [k9s](https://k9scli.io/) - Kubernetes CLI tool with full VIM bindings

* [DBeaver](https://dbeaver.io/) - Free Universal Database Tool
  * :heavy\_plus\_sign: [Vrapper plugin](https://vrapper.sourceforge.net/home/) - Plugin adds vim bindings to SQL editor. Install it using instructions from <https://github.com/dbeaver/dbeaver/issues/8219> ⭐ 51,577 | 🐛 3,364 | 🌐 Java | 📅 2026-08-28

## E-Mail

* :white\_check\_mark: [sup](https://sup-heliotrope.github.io/) - a console-based email client for people with a lot of email with Vim-inspired [keyboard shortcuts](https://github.com/sup-heliotrope/sup/wiki/Keyboard-reference) ⭐ 970 | 🐛 73 | 🌐 Ruby | 📅 2026-07-19.
* :white\_check\_mark: [Mutt](http://www.mutt.org/) - The vim of email, a TUI email client
* :white\_check\_mark: [NeoMutt](https://neomutt.org/) - A fork of mutt, intended to reignite the development.
* [Thunderbird](https://www.thunderbird.net/en-US/)
  * :heavy\_plus\_sign: ~~[teledactyl](https://github.com/5digits/dactyl/tree/master/teledactyl) ⭐ 467 | 🐛 105 | 🌐 JavaScript | 📅 2017-06-16~~
  * :heavy\_plus\_sign: ~~[Muttator](https://addons.thunderbird.net/en-US/thunderbird/addon/muttator/)~~ - Like Vimperator but for thunderbird.
* :white\_check\_mark: [aerc](https://aerc-mail.org/) - Terminal email client with Vim keybindings.
* :white\_check\_mark: [meli](https://meli.delivery/) - A TUI email client with Vim-like keybindings.
* Microsoft Outlook
  * :heavy\_plus\_sign: ~~[cubiclevim](https://sourceforge.net/projects/cubiclevim/)~~ - Edit Microsoft Outlook messages in Vim-style.

## Economy

* :white\_check\_mark: [cointop](https://github.com/cointop-sh/cointop) ⚠️ Archived - interactive terminal-based UI application for tracking and monitoring cryptocurrency.

## File Management

* :white\_check\_mark: [nnn](https://github.com/jarun/nnn) ⭐ 21,842 | 🐛 4 | 🌐 C | 📅 2026-08-29 - TUI file manager.
* :white\_check\_mark: [ranger](https://github.com/ranger/ranger) ⭐ 17,374 | 🐛 898 | 🌐 Python | 📅 2026-08-15 - Another TUI file manager.
* :white\_check\_mark: [lf](https://github.com/gokcehan/lf) ⭐ 9,481 | 🐛 81 | 🌐 Go | 📅 2026-08-25 - TUI file manager similar to ranger.
* :white\_check\_mark: [xplr](https://github.com/sayanarijit/xplr) ⭐ 4,813 | 🐛 13 | 🌐 Rust | 📅 2026-08-25 - TUI file manager.
* :white\_check\_mark: [felix](https://github.com/kyoheiu/felix) ⭐ 915 | 🐛 29 | 🌐 Rust | 📅 2025-04-12 - TUI file manager.
* :white\_check\_mark: [cfiles](https://github.com/mananapr/cfiles) ⭐ 508 | 🐛 22 | 🌐 C | 📅 2021-08-28 - A ncurses file manager written in C with Vim-like keybindings.
* :white\_check\_mark: ~~[vide](https://github.com/xaizek/vide) ⭐ 2 | 🐛 0 | 🌐 C | 📅 2014-05-18~~ - The graphical predecessor of vifm that uses GTK+
* :white\_check\_mark: [vifm](https://vifm.info/) - TUI file manager with vi keybindings.
* :white\_check\_mark: [ncdu](https://dev.yorhel.nl/ncdu) - ncurses disk usage explorer.
* :white\_check\_mark: [rover](http://lecram.github.io/p/rover/) - A small file browser with Vi-like key bindings for navigation.
* :white\_check\_mark: [broot](https://dystroy.org/broot/) - An interactive file tree explorer. [vim\_mode](https://dystroy.org/broot/vim_mode/) can be enabled in the configuration file.
* [Total Commander](https://www.ghisler.com/)
  * :heavy\_plus\_sign: [ViATc](https://github.com/magicstep/ViATc-English) ⭐ 32 | 🐛 2 | 🌐 AutoHotkey | 📅 2021-12-25 - adds a Vim mode to Total Commander.
* macOS Finder
  * :heavy\_plus\_sign: [Finder Vim Mode](https://github.com/chrisgrieser/finder-vim-mode) ⭐ 128 | 🐛 0 | 🌐 Shell | 📅 2026-08-03 - adds extensive vim-like/ranger-like keybindings, works via Karabiner Elements.
* :white\_check\_mark: ~~[jvifm](https://sourceforge.net/projects/jvifm/)~~ - A Java implementation of vifm; a file manager with Vim-like keybindings.
* [fman](https://fman.io/) - A dual-pane file manager.
  * :heavy\_plus\_sign: [VimNavigation](https://github.com/raguay/VimNavigation) - Adds Vim-style keyboard navigation to the fman file manager.
* :white\_check\_mark: [yazi](https://yazi-rs.github.io/) - Blazing fast terminal file manager written in Rust, based on async I/O.
* :white\_check\_mark: [superfile](https://superfile.dev/) - Pretty fancy and modern terminal file manager that supports h-j-k-l out of the box. See also more vim-like configuration [here](https://superfile.dev/configure/custom-hotkeys/#vim-like-superfile-hotkeys).

## IDEs

* [Jetbrain's IDEs](https://www.jetbrains.com/products/#type=ide) (Intellij, PYCharm, PHPStorm, WebStorm, ...)
  * :heavy\_plus\_sign: [IdeaVim](https://plugins.jetbrains.com/plugin/164-ideavim) - Install it directly from the plugin section in the IDE settings.
* [Visual Studio Code (VSCode)](https://code.visualstudio.com/)
  * :heavy\_plus\_sign: [VSCodeVim](https://marketplace.visualstudio.com/items?itemName=vscodevim.vim) - Vim emulation for Visual Studio Code. [GitHub](https://github.com/VSCodeVim/Vim) ⭐ 15,201 | 🐛 1,906 | 🌐 TypeScript | 📅 2026-08-28
  * :heavy\_plus\_sign: [VSCode Neovim](https://marketplace.visualstudio.com/items?itemName=asvetliakov.vscode-neovim) - Alternative to the VIM plugin, uses a full nvim instance in the background instead of just emulating VIM. [GitHub](https://github.com/vscode-neovim/vscode-neovim) ⭐ 7,730 | 🐛 94 | 🌐 TypeScript | 📅 2026-07-21
* :white\_check\_mark: [XCode](https://developer.apple.com/xcode/) - Apple's IDE. Vim mode can be enabled under the "Editor" menu without the use of plugins.
  * :heavy\_plus\_sign: ~~[XVim](https://github.com/XVimProject/XVim) ⭐ 5,121 | 🐛 305 | 🌐 Objective-C | 📅 2018-01-09~~ plugin. Deprecated, use native keybindings (above) instead.
  * :heavy\_plus\_sign: ~~[XVim2](https://github.com/XVimProject/XVim2) ⭐ 2,286 | 🐛 98 | 🌐 Objective-C | 📅 2023-01-14~~ plugin. Deprecated, use native keybindings (above) instead.
* [Eclipse](https://www.eclipse.org/ide/)
  * :heavy\_plus\_sign: [vrapper-vim](https://marketplace.eclipse.org/content/vrapper-vim) - A wrapper that provides a Vim-like input scheme for moving around and editing text.
  * :heavy\_plus\_sign: [viplugin](https://marketplace.eclipse.org/content/viplugin)
  * :heavy\_plus\_sign: [viable](https://marketplace.eclipse.org/content/viable-vim-eclipse)
  * :heavy\_plus\_sign: ~~[vimplugin](https://sourceforge.net/projects/vimplugin/)~~
* [NetBeans](https://netbeans.apache.org/) - Java IDE
  * :heavy\_plus\_sign: [jVI](https://jvi.sourceforge.net/) - A Vim-editor clone for the NetBeans IDE.
  * :heavy\_plus\_sign: ~~[viex](https://sourceforge.net/projects/viex/)~~
* [Visual Studio](https://visualstudio.microsoft.com/)
  * :heavy\_plus\_sign: [VsVim (Visual Studio 2015-2019)](https://marketplace.visualstudio.com/items?itemName=JaredParMSFT.VsVim) - install through the extensions inside Visual Studio
  * :heavy\_plus\_sign: [VsVim 2022 (Visual Studio 2022)](https://marketplace.visualstudio.com/items?itemName=JaredParMSFT.VsVim2022Preview) - install through the extensions inside Visual Studio
  * :heavy\_plus\_sign: [viemu](http://www.viemu.com/) - add Vim emulation to Visual Studio, SQL Server, Word & Outlook.
* [Geany](https://www.geany.org/)
  * :heavy\_plus\_sign: [vimode](https://github.com/geany/geany-plugins/blob/master/vimode/README) ⭐ 644 | 🐛 337 | 🌐 C | 📅 2026-07-11 - The vimode plugin can be enabled from the settings.
* :white\_check\_mark: [KDevelop](https://www.kdevelop.org/) - Uses the same editor component as Kate. Enable [Vi-mode](https://docs.kde.org/stable5/en/kate/katepart/vi-input-mode-chapter.html) in the editor settings.
* :white\_check\_mark: [Qt Creator](https://www.qt.io/product/development-tools) - Vim mode is built-in. Enable [FakeVim](https://doc.qt.io/qtcreator/creator-reference-preferences-fakevim.html) via Preferences > FakeVim.
* :white\_check\_mark: [RStudio](https://posit.co/download/rstudio-desktop/) - There's a built-in [Vim Editing Mode](https://stackoverflow.com/a/47208291).
* :white\_check\_mark: [MonoDevelop](https://www.monodevelop.com/) - Cross platform IDE for C#, F# and more, with [Vi-mode](https://www.monodevelop.com/archived/developers/tasks/source-editing/vi-mode/).
* :white\_check\_mark: ~~[pida](https://launchpad.net/pida)~~ - An IDE that aims to use the tools you wish to use(including Vim and Emacs).
* DrRacket - IDE for learning the Racket language.
  * :heavy\_plus\_sign: ~~[DrRacket Vim Tool](https://github.com/takikawa/drracket-vim-tool) ⭐ 216 | 🐛 40 | 🌐 Racket | 📅 2025-09-20~~ - An IDE that aims to use the tools you wish to use(including Vim and Emacs).
* :white\_check\_mark: [Zed](https://zed.dev/) - Vim mode is built-in. Can be [enabled](https://zed.dev/docs/configuring-zed#vim) and [configured](https://zed.dev/docs/vim) in the settings file.

## Image Editors

* :white\_check\_mark: [rx](https://rx.cloudhead.io/) - A pixel editor.
* :white\_check\_mark: [ViPaint](https://gitlab.com/jgkamat/ViPaint) - A modal Vi-like painting program.

## Image Viewers

* :white\_check\_mark: ~~[sxiv](https://github.com/xyb3rt/sxiv) ⚠️ Archived~~ - See nsxiv instead.
* :white\_check\_mark: ~~[vimiv](https://github.com/karlch/vimiv) ⭐ 299 | 🐛 13 | 🌐 Python | 📅 2020-06-16~~ - See vimiv-qt.
* :white\_check\_mark: [vimiv-qt](https://github.com/karlch/vimiv-qt) ⭐ 201 | 🐛 61 | 🌐 Python | 📅 2024-08-10 - An image viewer with Vim-like keybindings.
* :white\_check\_mark: [Pim](https://github.com/Narrat/Pim) ⭐ 29 | 🐛 7 | 🌐 Python | 📅 2021-03-31 - A PyGObject-based image viewer with Vim-like keybindings.
* :white\_check\_mark: [xzgv](https://sourceforge.net/projects/xzgv/) - Keyboard driven image viewer with Vim-style navigation.
* :white\_check\_mark: [imv](https://sr.ht/~exec64/imv/) - A command-line image viewer intended for use with tiling window managers (X11/Wayland).
* :white\_check\_mark: [nsxiv](https://codeberg.org/nsxiv/nsxiv) - A maintained fork of sxiv.

## Hex editors

* :white\_check\_mark: [hx](https://github.com/krpors/hx) ⭐ 210 | 🐛 1 | 🌐 C | 📅 2024-08-03 - Hex editor for the terminal with simple Vim-like keybindings.
* :white\_check\_mark: ~~[HEdit](https://github.com/95ulisse/hedit) ⭐ 3 | 🐛 0 | 🌐 C | 📅 2018-05-10~~ - A Vim-like terminal-based hex editor scriptable with JS.
* :white\_check\_mark: [bvi](https://bvi.sourceforge.net/) - A Hex editor for those familiar with Vi-like keybindings
* :white\_check\_mark: [hed](https://repo.or.cz/w/hed.git) - A terminal hexadecimal editor with Vim-like controls.
* :white\_check\_mark: [hexer](https://devel.ringlet.net/editors/hexer/) - a Vi-like binary editor.
* :white\_check\_mark: ~~[bviplus](https://bviplus.sourceforge.net/)~~ - An ncurses based Gex editor with a Vim-like interface.

## Misc

* :white\_check\_mark: [glow](https://github.com/charmbracelet/glow) ⭐ 27,104 | 🐛 225 | 🌐 Go | 📅 2026-08-16 - Terminal based markdown reader.
* :white\_check\_mark: [fx](https://github.com/antonmedv/fx) ⭐ 20,603 | 🐛 26 | 🌐 Go | 📅 2026-08-26 - Terminal based JSON viewer.
* :white\_check\_mark: [gollum](https://github.com/gollum/gollum) ⭐ 14,319 | 🐛 91 | 🌐 Ruby | 📅 2025-11-24 - A Git-powered wiki with built-in Vim editing mode. Start with `--default-keybind vim`.
* :white\_check\_mark: [ly](https://github.com/fairyglade/ly) ⭐ 7,549 | 🐛 0 | 🌐 Zig | 📅 2026-08-27 - A TUI display manager. Supports vi-like movement. Edit this in your `/etc/ly/config.ini`

  * ```ini
    # Default vi mode
    # normal   -> normal mode
    # insert   -> insert mode
    vi_default_mode = normal

    # Enable vi keybindings
    vi_mode = true
    ```
* :white\_check\_mark: [mdp](https://github.com/visit1985/mdp) ⭐ 5,276 | 🐛 12 | 🌐 C | 📅 2025-07-09 - A command-line based markdown presentation tool.
* :white\_check\_mark: [pulsemixer](https://github.com/GeorgeFilipkin/pulsemixer) ⭐ 808 | 🐛 36 | 🌐 Python | 📅 2024-03-14 - CLI and curses mixer for [PulseAudio](https://www.freedesktop.org/wiki/Software/PulseAudio/).
* :white\_check\_mark: [stig](https://github.com/rndusr/stig) ⭐ 629 | 🐛 53 | 🌐 Python | 📅 2026-01-24 - TUI/CLI for the BitTorrent client Transmission.
* :white\_check\_mark: [sentaku](https://github.com/rcmdnk/sentaku) ⭐ 150 | 🐛 3 | 🌐 Shell | 📅 2026-07-20 - A terminal selector with Vim-like keybindings.
* :white\_check\_mark: ~~[Yzis](https://github.com/chrizel/Yzis) ⭐ 44 | 🐛 3 | 🌐 C++ | 📅 2017-11-16~~ - A vi/vim engine that is easy to integrate in any graphical application.
* :white\_check\_mark: [Foliate](https://johnfactotum.github.io/foliate/) - An e-book reader with basic vim-like navigation
* :white\_check\_mark: [pipedial](https://code.reversed.top/user/xaizek/pipedial) - A terminal selector with basic Vim-like keybindings.
* :white\_check\_mark: [termshark](https://termshark.io/) - a UI for tshark with Vim-navigation.
* :white\_check\_mark: [mycli](https://www.mycli.net) - A CLI for MySQL, MariaDB, and Percona with auto-completion and syntax highlighting. There are two types of keybindings available. Emacs mode and Vi mode.
* [Anki](https://apps.ankiweb.net/) - Spaced repetition and media-rich cards flashcard program for study.
  * ➕ [anki\_vimove](https://ankiweb.net/shared/info/1997961715) - Add-on for vi-like movement in deck browser.

## Music Players

* :white\_check\_mark: [cmus](https://github.com/cmus/cmus) ⭐ 6,227 | 🐛 219 | 🌐 C | 📅 2026-08-12 - A console music player with vim-like [keybindings](https://man.archlinux.org/man/cmus.1.en#KEYBINDINGS).
* :white\_check\_mark: [ncmpcpp](https://github.com/ncmpcpp/ncmpcpp) ⭐ 2,476 | 🐛 226 | 🌐 C++ | 📅 2026-06-25 - An ncurses client for [mpd](https://www.musicpd.org/). The navigation can quite easily be made to behave like vim with some keyboard configurations.
  * <details>
      <summary>~/.config/ncmpcpp/bindings</summary>

    ```
    def_key "j"
      scroll_down
    def_key "k"
      scroll_up
    def_key "h"
      previous_column
    def_key "l"
      next_column
    def_key "ctrl-b"
      page_up
    def_key "ctrl-u"
      page_up
    def_key "ctrl-f"
      page_down
    def_key "ctrl-d"
      page_down
    def_key "g"
      move_home
    def_key "G"
      move_end
    def_key "n"
      next_found_item
    def_key "N"
      previous_found_item
    ```

    </details>
* :white\_check\_mark: [vimpc](https://github.com/boysetsfrog/vimpc) ⭐ 281 | 🐛 21 | 🌐 C++ | 📅 2023-06-14 - A console mpd client that provides a vim-like interface. Default keybindings in the [help file](https://github.com/boysetsfrog/vimpc/blob/master/doc/help.txt) ⭐ 281 | 🐛 21 | 🌐 C++ | 📅 2023-06-14
* :white\_check\_mark: [vimus](https://github.com/vimus/vimus) ⭐ 138 | 🐛 20 | 🌐 Haskell | 📅 2022-07-13 - An MPD client with Vim-like keybindings.
* :white\_check\_mark: ~~[herrie](https://github.com/EdSchouten/herrie) ⚠️ Archived~~ - a MPD player with Vim-like [keybindings](https://github.com/EdSchouten/herrie/blob/master/herrie/man/00-man) ⚠️ Archived.
* :white\_check\_mark: [vitunes](http://vitunes.org/) - An MPD client with Vi-like bindings.
* :white\_check\_mark: [pms](https://kimtore.github.io/pms/) - A frontend to MPD with Vim-like keybindings.
* :white\_check\_mark: [siren](https://www.kariliq.nl/siren/) - A text-based audio player with [Vim-like](https://www.kariliq.nl/man/siren.1.html) keybindings.
* YT Music
  * :white\_check\_mark: [vimyt](https://github.com/Sadoaz/vimyt) ⭐ 41 | 🐛 1 | 🌐 Go | 📅 2026-06-28 – TUI for YouTube Music with Vim-like keybindings.
* Spotify
  * :white\_check\_mark: [spotify-tui](https://github.com/Rigellute/spotify-tui) ⭐ 19,331 | 🐛 306 | 🌐 Rust | 📅 2024-04-04 - TUI for Spotify with Vim-like keybindings.
  * :heavy\_plus\_sign: [spicetify](https://spicetify.app/) - an extension framework for spotify. Includes an extension with [vim-like](https://spicetify.app/docs/advanced-usage/extensions/#keyboard-shortcut) keybindings.

## Music Production

* :heavy\_plus\_sign: [Reaper-Keys](https://github.com/gwatcha/reaper-keys) ⭐ 201 | 🐛 1 | 🌐 Lua | 📅 2026-07-05 - Bringing a modal editor to the Reaper DAW.
* :white\_check\_mark: ~~[pineapple-tracker](https://github.com/pineapple-tracker/pineapple-tracker) ⭐ 32 | 🐛 2 | 🌐 C | 📅 2026-06-10~~ - A console-based sequencer with a vi-style UI.
* [Reaper](https://www.reaper.fm/) - A DAW.

## News/RSS Readers

* :heavy\_plus\_sign: ~~[Newsbeuter](https://github.com/akrennmair/newsbeuter) ⚠️ Archived~~ - Unmaintained, see Newsboat./
* :heavy\_plus\_sign: [Newsboat](https://newsboat.org/) - RSS/Atom reader with a TUI.

## Office Productivity

* :white\_check\_mark: [sc-im](https://github.com/andmarti1424/sc-im) ⭐ 5,692 | 🐛 117 | 🌐 C | 📅 2026-08-26 - Like sc but improved, a Vim-like spreadsheet calculator.
* [LibreOffice](https://www.libreoffice.org/)
  * :heavy\_plus\_sign: ~~[vibreoffice](https://github.com/seanyeh/vibreoffice) ⚠️ Archived~~ - Vi Mode for LibreOffice/OpenOffice.
  * :heavy\_plus\_sign: [vibreoffice](https://github.com/Nazo1412/vibreoffice) ⭐ 16 | 🐛 0 | 🌐 VBScript | 📅 2022-11-20 - Vi Mode for LibreOffice/OpenOffice, fork that supports calc.
* [AbiWord](http://www.abisource.com/) - An OSS word processor.
  * :heavy\_plus\_sign: It can be [configured](http://recycledelectron.blogspot.com/2009/01/vi-and-emacs-key-bindings-in-abiword.html) to get Vim keybindings.
* :white\_check\_mark: [sc](https://en.wikipedia.org/wiki/Sc_\(spreadsheet_calculator\)) - The venerable Spreadsheet Calculator with Vim-like [keybindings](https://www.linuxjournal.com/article/10699).
* :white\_check\_mark: [VisiData](https://www.visidata.org/) - A TUI data exploration tool with Vim-like [navigation](https://jsvine.github.io/intro-to-visidata/basics/navigating-visidata/).
* Google Docs Editors suite
  * :heavy\_plus\_sign: [SheetKeys](https://github.com/philc/sheetkeys) ⭐ 333 | 🐛 30 | 🌐 JavaScript | 📅 2026-02-26 - Browser extension (Chrome and Firefox) which adds Vim keybindings to Google Sheets.

## Pagers

* :white\_check\_mark: [bat](https://github.com/sharkdp/bat) ⭐ 60,289 | 🐛 424 | 🌐 Rust | 📅 2026-08-11
* :white\_check\_mark: [less](https://en.wikipedia.org/wiki/Less_\(Unix\))

## PDF Viewers

* :white\_check\_mark: [Sioyek](https://github.com/ahrm/sioyek) ⭐ 9,809 | 🐛 324 | 🌐 C | 📅 2026-08-18 - Both keyboard and (optionally) mouse focused. Configurable and has the possibility of adding and developing plugins.
* :white\_check\_mark: [apvlv](https://github.com/naihe2010/apvlv) ⭐ 259 | 🐛 16 | 🌐 C++ | 📅 2026-07-31 - A PDF Viewer that acts Like Vim
* :white\_check\_mark: [MuPDF](https://mupdf.com) - PDF and ebook reader with [vim keybindings](http://tuxdiary.com/2015/04/18/mupdf/).
* :white\_check\_mark: [zathura](https://pwmt.org/projects/zathura) - Document reader, vim-keybindings, partly based on MuPDF. Linux only.
* :white\_check\_mark: [SumatraPDF](https://www.sumatrapdfreader.org/free-pdf-reader) - Document reader, vim-keybindings. Windows only.
* :white\_check\_mark: [Okular](https://okular.kde.org/) - Has some [basic](https://docs.kde.org/stable5/en/okular/okular/okular.pdf) Vim-like navigation.
* :white\_check\_mark: [Evince](https://gitlab.gnome.org/GNOME/evince) - Has some basic Vim-like navigation.
* :white\_check\_mark: [xpdf](https://www.xpdfreader.com/) - This PDF viewer can be [configured](https://stackoverflow.com/a/11800265/265508) to get Vim-like navigation.
* Preview\.app - macOS native document viewer:
  * :heavy\_plus\_sign: [preview-vim](https://github.com/xrisk/preview-vim) ⭐ 56 | 🐛 1 | 📅 2021-01-24 - Adds vim-like keybindings, works via Karabiner Elements.

## Personal Knowledge Management

* :white\_check\_mark: [Trilium](https://github.com/zadam/trilium) ⭐ 37,626 | 🐛 709 | 🌐 TypeScript | 📅 2026-08-29 - 'Enable Vim Keybindings' added to Options in early-2022
  * code notes use the [CodeMirror](https://github.com/codemirror/dev/) ⚠️ Archived editor and its [Vim mode](https://codemirror.net/5/demo/vim.html)
* :white\_check\_mark: [Obsidian](https://obsidian.md/) - under "Editor" options
* [Logseq](https://logseq.com/)
  * :heavy\_plus\_sign: [logseq-plugin-vim-shortcuts](https://github.com/vipzhicheng/logseq-plugin-vim-shortcuts) ⭐ 407 | 🐛 22 | 🌐 TypeScript | 📅 2025-12-27 - normal mode commands deal with whole blocks, editing text is only possible in edit mode
* :white\_check\_mark: [Joplin](https://joplinapp.org/) - under "Tools" → "Options" → "General" → "Show Advanced Settings" → "Keyboard Mode"

## Social

* ~~[rtv](https://github.com/michael-lazar/rtv) ⚠️ Archived~~ - A Reddit TUI viewer
* :white\_check\_mark: [iamb](https://github.com/ulyssa/iamb) ⭐ 1,269 | 🐛 169 | 🌐 Rust | 📅 2026-08-23 - A Matrix client for Vim addicts.
* :white\_check\_mark: [scli](https://github.com/isamert/scli) ⭐ 538 | 🐛 26 | 🌐 Python | 📅 2024-11-30 - Signal messenger TUI with Vim-like keybindings.
* :white\_check\_mark: [tut](https://github.com/RasmusLindroth/tut) ⭐ 500 | 🐛 56 | 🌐 Go | 📅 2023-12-18 - a Mastodon client with vim-like navigation
* [irssi](https://github.com/shabble/irssi-scripts/tree/master/vim-mode) ⭐ 151 | 🐛 19 | 🌐 Perl | 📅 2021-07-17 - the popular IRC client.
  * :heavy\_plus\_sign: [vim\_mode](https://github.com/shabble/irssi-scripts/tree/master/vim-mode) ⭐ 151 | 🐛 19 | 🌐 Perl | 📅 2021-07-17 plugin.
* :white\_check\_mark: [matui](https://github.com/pkulak/matui) ⭐ 121 | 🐛 0 | 🌐 Rust | 📅 2026-07-29 - a Matrix TUI with vim-like navigation.
* [weechat](https://weechat.org/) - A flexible IRC client.
  * :heavy\_plus\_sign: [weechat-vimode](https://github.com/GermainZ/weechat-vimode) ⭐ 276 | 🐛 14 | 🌐 Python | 📅 2025-04-27 - A script that will configure Weechat to get Vim-like navigation.
* ~~[vchatter](https://vchatter.sourceforge.net/)~~ - A Vi-like Jabber chat client.

## Source Code Management

* :white\_check\_mark: [Lazygit](https://github.com/jesseduffield/lazygit) ⭐ 81,737 | 🐛 1,024 | 🌐 Go | 📅 2026-08-27 - Simple terminal UI for git commands with Vim-like keybindings.

* :white\_check\_mark: [GitUI](https://github.com/extrawurst/gitui) ⭐ 22,445 | 🐛 343 | 🌐 Rust | 📅 2026-08-04 - GitUI provides you with the comfort of a git GUI but right in your terminal.
  * instruction how to enable vi bindings - <https://github.com/extrawurst/gitui/blob/master/KEY_CONFIG.md> ⭐ 22,445 | 🐛 343 | 🌐 Rust | 📅 2026-08-04

* :white\_check\_mark: [tig](https://jonas.github.io/tig/) - Text interface for git. Works mostly like vim out of the box, but can be enhanced by sourcing these [keybindings](https://github.com/jonas/tig/blob/master/contrib/vim.tigrc) ⭐ 13,318 | 🐛 232 | 🌐 C | 📅 2026-07-27 in your `~/.tigrc`.

* :white\_check\_mark: [git](https://git-scm.com/) - Nothing's better than the real deal. Tell git to use vim/nvim when editing commit messages, interactive rebase, etc. by putting in your `~/.config/git/config`:

  * ```ini
    [user]
        editor = vim
    ```

* :white\_check\_mark: [hg/mercurical](https://www.mercurial-scm.org/) - Put in your `~/.config/hg/hgrc`:

  * ```ini
    [ui]
        editor = vim
    ```

## Search Engines

* :white\_check\_mark: [searxng](https://docs.searxng.org/) - SearXNG is a free internet metasearch engine which aggregates results from various search services and databases. Users are neither tracked nor profiled. You can either enable vi binds in the settings when using the site or when selfhosting, you can set the default hotkeys to be vi styled for every user.

  * Preferences > USER INTERFACE > Hotkeys
  * <details>
    <summary>Server configuration at /etc/searxng/settings.yml</summary>

    ```
    ui:
      hotkeys: vim
    ```

  </details>

* :white\_check\_mark: [DuckDuckGo](https://duckduckgo.com/) - DuckDuckGo lets you search and browse privately, it never tracks you. It has some vim-like bindings by default in its [keyboard shortcuts](https://duckduckgo.com/duckduckgo-help-pages/features/keyboard-shortcuts).

* :white\_check\_mark: [Kagi](https://kagi.com/) - Kagi is a paid ad-free search engine that has vim-like bindings by default in its [keyboard shortcuts](https://help.kagi.com/kagi/features/search-operators.html#keyboard_shortcuts).

## Shells

* :white\_check\_mark: [readline](https://man.archlinux.org/man/readline.3) - Readline is a library used by many CLI programs to read input from users. By configuring readline to use vi key bindings, you automatically get it for programs like `bash`, `irb`, `octave`, etc. By default, readline has Emacs-like keybindings, but you can change that by putting this in your `~/.inputrc`:

  * ```
    set editing-mode vi
    set keymap vi-insert
    ```

* :white\_check\_mark: [Bash](https://www.gnu.org/software/bash/) - The preferred method is to set Vi mode in `~/.inputrc` via readline, as you will get Vi mode automatically in all programs using the library. However, if you just want this for bash, put this in your bash startup file e.g., `~/.bashrc`:

  * :heavy\_plus\_sign: [ble.sh](https://github.com/akinomyoga/ble.sh) ⭐ 4,653 | 🐛 84 | 🌐 Shell | 📅 2026-08-18 (Bash Line Editor) - An interactive plugin `ble.sh` provides a better Vim mode as well as syntax highlighting and autosuggestions.  In addition to the above setting of `set -o vi` in `~/.bashrc` or `set editing-mode vi` in `~/.inputrc`, you can add the following settings in `~/.bashrc` to enable `ble.sh`.

    * ```
      # bashrc

      # Add these lines at the top of .bashrc:
      [[ $- == *i* ]] && source /path/to/blesh/ble.sh --noattach

      # your bashrc settings come here...

      # Add this line at the end of .bashrc:
      [[ ! ${BLE_VERSION-} ]] || ble-attach
      ```

  * ```bash
    set -o vi
    ```

* :white\_check\_mark: [zsh](https://en.wikipedia.org/wiki/Z_shell) - just put this in your ZSH startup file, most likely `~/.zshrc`:

  * :heavy\_plus\_sign: [zsh-vi-mode](https://github.com/jeffreytse/zsh-vi-mode) ⭐ 4,435 | 🐛 130 | 🌐 Shell | 📅 2026-07-19 - A better and friendlier Vim-mode plugin for zsh.

  * ```bash
    bindkey -v
    ```

  * <details>
      <summary>Extra text object keybindings</summary>

    ```bash
    # Add text object extension -- eg ci" da(:
    autoload -U select-quoted
    zle -N select-quoted
    for m in visual viopp; do
        for c in {a,i}{\',\",\`}; do
            bindkey -M $m $c select-quoted
        done
    done
    ```

    </details>

* :white\_check\_mark: [fish](https://fishshell.com/) - Just add to your `~/.config/fish/config.fish` ([reference](https://stackoverflow.com/a/28445450/265508)):

  * ```bash
    fish_vi_key_bindings
    ```

* :white\_check\_mark: [tcsh](https://www.tcsh.org/) - Put this in your tcsh startup file e.g. `~/.tcshrc` ([reference](https://www.oreilly.com/library/view/mac-os-x/0596004583/ch04s02.html)):

  * ```bash
    bindkey -v
    ```

* :white\_check\_mark: [ksh](https://en.wikipedia.org/wiki/KornShell) - Put this in your ksh startup file e.g. `~/.kshrc`:

  * ```bash
    set -o vi
    ```

* :white\_check\_mark: [nushell](https://www.nushell.sh) - Put this in your config file e.g. `$nu.config-path`:

  * ```nu
    let-env config = {
      # ...
      edit_mode: vi,
      # ...
    }
    ```

* ✅ [pwsh](https://learn.microsoft.com/en-us/powershell/) - The Readline module offers support for convenient vim support. Add this to your `$Profile`:
  * <details>
      <summary>$PROFILE</summary>

    ```powershell
    Import-Module PSReadLine
    # enable Vim on the shell and as editor
    $OnViModeChange = [scriptblock]{
        if ($args[0] -eq 'Command') {
            # Set the cursor to a blinking block.
            Write-Host -NoNewLine "`e[2 q"
        }
        else {
            # Set the cursor to a blinking line.
            Write-Host -NoNewLine "`e[5 q"
        }
    }

    Set-PsReadLineOption -EditMode Vi
    Set-PSReadLineOption -ViModeIndicator Script -ViModeChangeHandler $OnViModeChange
    ```

    </details>
  *
  * This was collected from many GitHub issues and posts. PowerShell 5.1, for one reason or another, refuses to change the cursor, so the script to give
    feedback does not work. Just remove it, and it will still work, just no feedback of the mode you're in.

* :white\_check\_mark: [xonsh](https://xon.sh/) - Put this in your run control file `~/.xonshrc`:

  * ```
     $VI_MODE = True
    ```

## System-wide

* :white\_check\_mark: [vim-anywhere](https://github.com/cknadler/vim-anywhere) ⭐ 3,767 | 🐛 44 | 🌐 Shell | 📅 2026-05-02 - Spawn a Vim buffer from any text input in the operating system.
* :white\_check\_mark: [warpd](https://github.com/rvaiya/warpd) ⭐ 3,622 | 🐛 108 | 🌐 C | 📅 2024-07-12 - A modal keyboard-driven interface for mouse manipulation, Linux (X11/Wayland)
* :white\_check\_mark: [win-vind](https://github.com/pit-ray/win-vind) ⚠️ Archived - Control the Windows GUI in the same way as Vim.
* :white\_check\_mark: [athame](https://github.com/ardagnir/athame) ⭐ 1,654 | 🐛 23 | 🌐 C | 📅 2023-11-01 - Patches your shell to add full Vim support by routing your keystrokes through an actual Vim process.
* :white\_check\_mark: [Hints](https://github.com/AlfredoSequeida/hints) ⭐ 1,354 | 🐛 18 | 🌐 Python | 📅 2026-06-28 - Navigate GUI applications in Linux without your mouse by displaying "hints" you can type on your keyboard to interact with GUI elements (X11/Wayland)
* :white\_check\_mark: [sketchyvim](https://github.com/FelixKratz/SketchyVim) ⭐ 1,021 | 🐛 26 | 🌐 C | 📅 2024-03-16 - Get vim-like navigation in any macOS text field.
* :white\_check\_mark: [keystrokes](https://github.com/Darukutsu/keystrokes) ⭐ 2 | 🐛 2 | 🌐 Shell | 📅 2025-01-30 - Record your keystrokes and replay them just like in Vim macro, Linux (X11/Wayland)
* :white\_check\_mark: [Homerow](https://www.homerow.app/) - Add vim-like navigation to any macOS app.
* :white\_check\_mark: [kindaVim](https://kindavim.app/) - Get Vim motions all over macOS, in text fields, text areas, and other UI elements.
* :white\_check\_mark: [Scrolla](https://scrolla.app/) - Scroll in macOS using Vim motions.
* :white\_check\_mark: ~~[kommand](https://www.autohotkey.com/board/topic/42706-kommand-a-cross-application-vim-like-hot-key-solution/)~~ - A cross-application Vim-like hot key solution.
* :white\_check\_mark: [AltTab](https://alt-tab-macos.netlify.app/) - A utility that brings Windows-style Alt-Tab functionality to macOS with Vim key support.  To enable Vim keys, go to:  `Preferences` → `Controls` → `Additional controls` → **Select windows using Vim keys**.

## System Tools

* :white\_check\_mark: [btop++](https://github.com/aristocratos/btop) ⭐ 34,284 | 🐛 534 | 🌐 C++ | 📅 2026-08-26 - A resource monitor. To enable Vim navigation, set in the config file:

  * ```ini
    vim_keys = True
    ```

* :white\_check\_mark: [CopyQ](https://github.com/hluk/CopyQ) ⭐ 12,191 | 🐛 405 | 🌐 C++ | 📅 2026-08-23 - A clipboard manager with basic Vim-like navigation.

* :white\_check\_mark: [htop-vim](https://aur.archlinux.org/packages/htop-vim/) - A patched version the [htop](https://htop.dev/) interactive process viewer that has vim keybindings for navigation.

* :white\_check\_mark: [aptitude](https://wiki.debian.org/Aptitude) - ncurses interface for APT on Debian-derived Linux distros. The [keybindings](https://www.debian.org/doc/manuals/aptitude/ch02s05s02.en.html) are already vim-like.

* :white\_check\_mark: [lnav](https://lnav.org/) - A log viewer with minimal Vim-like [navigation](https://docs.lnav.org/en/latest/hotkeys.html).

## Task Management

* :white\_check\_mark: [vit](https://github.com/vit-project/vit) ⭐ 581 | 🐛 76 | 🌐 Python | 📅 2026-03-17 - An TUI for [Taskwarrior](https://taskwarrior.org/) Vim-like keybindings.
* :white\_check\_mark: [kabmat](https://github.com/PlankCipher/kabmat) ⭐ 425 | 🐛 13 | 🌐 C++ | 📅 2023-01-26 - TUI for managing kanban boards with Vim-like keybindings.
* :white\_check\_mark: [Keyban](https://site.keyban.app/) - Kanban board/task management/bullet journal app built for Vim-like operation.
* :white\_check\_mark: [TuDu](https://code.meskio.net/tudu/) - A command-line interface to manage hierarchical todos.
* :white\_check\_mark: [calcurse](https://calcurse.org/) - A calendar and scheduling application for the command line with default [vim-like keybindings](http://culot.org/calcurse/manual_en.html#options_keys).
* :white\_check\_mark: [taskell](https://taskell.app/) - Command-line Kanban board/task management.
* :white\_check\_mark: [Remember The Milk](https://www.rememberthemilk.com/help/answer/basics-basics-keyboard) - A task management application available on various platforms, including web, Windows, Linux, macOS desktop, and Android & iOS mobile apps. It offers built-in Vim-like keybindings on its desktop and web versions.

## Terminal Emulators

* :white\_check\_mark: [alacritty](https://github.com/alacritty/alacritty) ⭐ 65,545 | 🐛 338 | 🌐 Rust | 📅 2026-08-26 - A cross-platform, OpenGL terminal emulator with Vim-like keybindings by default.
* :white\_check\_mark: [tmux](https://github.com/tmux/tmux) ⭐ 48,889 | 🐛 33 | 🌐 C | 📅 2026-08-28 - the terminal multiplexer, superseding GNU Screen.
  * <details>
      <summary>~/.config/tmux/tmux.conf</summary>

    ```ini
     set-option -g status-keys vi  # Use Vi bindings in tmux command prompt.
     set-window-option -g mode-keys vi # Use Vi bindings in copy and choice mode.

     # Optional: some Vi-like navigation for smart pane switching.
     # NOTE this could override default keybindings like <prefix>-l.
     bind h select-pane -L
     bind j select-pane -D
     bind k select-pane -U
     bind l select-pane -R
    ```

    </details>
* :white\_check\_mark: ~~[Termine](https://github.com/thestinger/termite) ⚠️ Archived~~ - See alacritty instead.
* [rxvt-unicode](https://wiki.archlinux.org/title/rxvt-unicode) - The Unicode fork of the rxvt terminal emulator.
  * :heavy\_plus\_sign: [urxvt-vim-scrollback](https://github.com/ervandew/urxvt-vim-scrollback) ⚠️ Archived - Provides Vim-like scrollback mode and pasting.
* :white\_check\_mark: [Kitty](https://sw.kovidgoyal.net/kitty/) - The fast, feature-rich, GPU-based terminal emulator. Through its configuration, users can configure splitting and navigation to mimic the behavior of Vi.
  * <details>
      <summary>~/.config/kitty/kitty.conf</summary>

    ```
    # Jump around neighboring window Vi key binding
    map ctrl+shift+w>h neighboring_window left
    map ctrl+shift+w>l neighboring_window right
    map ctrl+shift+w>j neighboring_window down
    map ctrl+shift+w>k neighboring_window up

    map ctrl+shift+w>shift+h move_window left
    map ctrl+shift+w>shift+l move_window right
    map ctrl+shift+w>shift+j move_window down
    map ctrl+shift+w>shift+k move_window up

    # Create a new window, splitting the space used by the existing one so that
    # the two windows are placed one above the other
    map ctrl+shift+w>s launch --location=hsplit

    # Create a new window, splitting the space used by the existing one so that
    # the two windows are placed side by side
    map ctrl+shift+w>v launch --location=vsplit

    # Use nvim as the pager. Remove all ASCII formatting characters.
    scrollback_pager nvim --noplugin -c 'set buftype=nofile' -c 'set noswapfile' -c 'silent! %s/\%x1b\[[0-9;]*[sumJK]//g' -c 'silent! %s/\%x1b]133;[A-Z]\%x1b\\//g' -c 'silent! %s/\%x1b\[[^m]*m//g' -c 'silent! %s///g' -
    ```

    </details>

## Text Editors

We know that Vi-[clones](http://www.linfo.org/vi/clones.html)/derivatives have Vi(m) keybindings so let's skip those here (Vim, NeoVim, vile, elvis, nvi, vis, pyvim, jVi, ex-vi ...)

* :white\_check\_mark: [kakoune](https://github.com/mawww/kakoune) ⭐ 11,036 | 🐛 920 | 🌐 C++ | 📅 2026-08-19 - A modal text editor inspired by Vim-navigation.

* :white\_check\_mark: ~~[oni2 (onivim)](https://github.com/onivim/oni2) ⭐ 7,843 | 🐛 547 | 🌐 Reason | 📅 2022-08-17~~ - [Deprecated](https://github.com/onivim/oni2/issues/3861) ⭐ 7,843 | 🐛 547 | 🌐 Reason | 📅 2022-08-17.

* :white\_check\_mark: [vy](https://github.com/vyapp/vy) ⚠️ Archived - A Vim-like in python made from scratch.

* :white\_check\_mark: [rim](https://github.com/mathall/rim) ⭐ 632 | 🐛 8 | 🌐 Rust | 📅 2021-01-16 - The aspiring Vim-like text editor.

* :white\_check\_mark: ~~[editra](https://github.com/cjprecord/editra) ⭐ 6 | 🐛 135 | 🌐 Python | 📅 2019-11-15~~ - Developers Text Editor, with a Vi-mode.

* Emacs
  * :heavy\_plus\_sign: [doom emacs](https://github.com/doomemacs/doomemacs) ⭐ 22,629 | 🐛 491 | 🌐 Emacs Lisp | 📅 2026-08-28 - Configuration package that provides a similar experience to Spacemacs (including `evil-mode`. Also implements spacebar-as-leader-key.
  * :white\_check\_mark: [evil-mode](https://www.emacswiki.org/emacs/Evil) - Extensible vi layer for Emacs.
  * :heavy\_plus\_sign: [spacemacs](https://www.spacemacs.org/) - Emacs configuration package that improves the Emacs experience, including vim bindings via `evil-mode`. Features a vim-like leader (space) for common commands.
  * :heavy\_plus\_sign: ~~[Vimpulse](https://www.emacswiki.org/emacs/Vimpulse)~~ Deprecated, check out Evil.
  * :heavy\_plus\_sign: ~~[Vim Mode](https://www.emacswiki.org/emacs/VimMode)~~ Deprecated, check out Evil.

* :white\_check\_mark: [Sublime Text](https://www.sublimetext.com/) has a bult-in [Vintage mode](https://www.sublimetext.com/docs/vintage.html) that can be enabled.
  * :heavy\_plus\_sign: ~~[Vintageous](https://github.com/guillermooo/Vintageous) ⭐ 1,629 | 🐛 227 | 🌐 Python | 📅 2018-07-29~~
  * :heavy\_plus\_sign: [NeoVintageous](https://github.com/NeoVintageous/NeoVintageous) ⭐ 728 | 🐛 51 | 🌐 Python | 📅 2026-08-21 - An advanced Vim emulation layer.
  * :heavy\_plus\_sign: ~~[VintageEx](https://github.com/SublimeText/VintageEx) ⚠️ Archived~~
  * :heavy\_plus\_sign: ~~[Six](https://packagecontrol.io/packages/Six)~~

* QTextEdit/QPlainTextEdit
  * :heavy\_plus\_sign: [FakeVim](https://github.com/hluk/FakeVim) ⭐ 183 | 🐛 21 | 🌐 C++ | 📅 2026-08-22

* :white\_check\_mark: [amp](https://amp.rs/) - A modal terminal text.

* :white\_check\_mark: [moe](https://editor.moe/) - A modal text editor with a Vim-like mode.

* :white\_check\_mark: [kate](https://kate-editor.org/) - A text editor with a [Vi-mode](https://kate-editor.org/kate-vi-mode/).

* :white\_check\_mark: [Komodo Edit](https://www.activestate.com/products/komodo-edit/) - Has [Vi emulation](https://www.activestate.com/blog/komodos-vi-emulation/).

* :white\_check\_mark: [slickedit](https://www.slickedit.com/) - A Code editor with [Vim emulation](https://www.slickedit.com/images/stories/products/slickedit/emulation_charts/Vim_Emulation.pdf).

* :white\_check\_mark: [WinVi](https://winvi.de/en/) - A Windows text editor highly compatible with Vi.

* :white\_check\_mark: [VNote](http://app.vnote.fun/en_us/) - A note-taking editor with Vi mode and Vi-like navigation.

* :white\_check\_mark: [novelWriter](https://novelwriter.io/) - Plain text editor for novel writing with built-in [Vim mode navigation](https://novelwriter.io/docs/features/vim_mode.html)

* [Inkdrop](https://www.inkdrop.app/) - A Markdown note-taking app.
  * :heavy\_plus\_sign: [inkdrop-vim](https://github.com/inkdropapp/inkdrop-vim) ⭐ 110 | 🐛 4 | 🌐 TypeScript | 📅 2026-08-26 - Provides a Vim modal control for Inkdrop.

* :white\_check\_mark: [GNOME Text Editor](https://gitlab.gnome.org/GNOME/gnome-text-editor) - If it's [installed](https://askubuntu.com/a/1439846) with APT, enable the Vim mode by running this in a Terminal:

  * ```bash
    gsettings set org.gnome.TextEditor keybindings vim
    ```

* ~~Atom~~ - [Discontinued](https://github.blog/2022-06-08-sunsetting-atom/)
  * :heavy\_plus\_sign: ~~[atom-vim-mode-plus](https://github.com/t9md/atom-vim-mode-plus) ⭐ 1,388 | 🐛 127 | 🌐 CoffeeScript | 📅 2021-10-07~~
  * :heavy\_plus\_sign: ![atom-vim-mode-plus](https://github.com/atom/vim-mode)\~

## Web Apps

* :white\_check\_mark: [HackerRank](https://www.hackerrank.com/) - Coding challenges and interview preparation across multiple domains.
* :white\_check\_mark: [leetcode](https://leetcode.com/) - Algorithmic programming problem repository.
* :white\_check\_mark: [OnlineGDB](https://www.onlinegdb.com/) - Online compiler and debugger supporting many programming languages.
* :white\_check\_mark: [Godbolt](https://godbolt.org/) - An interactive compiler exploration website.
* :white\_check\_mark: [Rust Playground](https://play.rust-lang.org/) - The editor in the Rust playground has a Vim mode.
* :white\_check\_mark: [Svelte Playground](https://svelte.dev/playground/) - The editor in the Svelte playground has a Vim mode.

## Web browsers

* :white\_check\_mark: [nyxt](https://github.com/atlas-engineer/nyxt) ⭐ 11,009 | 🐛 145 | 🌐 Common Lisp | 📅 2026-02-26 - A keyboard-driven web browser inspired by Vim and Emacs.

* :white\_check\_mark: ~~[xombrero](https://github.com/conformal/xombrero) ⭐ 162 | 🐛 44 | 🌐 C | 📅 2016-11-26~~ - A minimalist web browser with vi-like keyboard commands.

* :white\_check\_mark: [wyeb](https://github.com/jun7/wyeb) ⭐ 124 | 🐛 11 | 🌐 C | 📅 2025-10-23 - A Vim-like webkit2gtk web browser.

* :white\_check\_mark: ~~[Vimprobable](https://github.com/ThomasAdam/vimprobable) ⭐ 21 | 🐛 0 | 🌐 C | 📅 2013-06-01~~

* :white\_check\_mark: ~~[dwb](https://github.com/diab0l/dwb) ⭐ 10 | 🐛 0 | 🌐 C | 📅 2015-11-18~~ - See qutebrowser instead.

* :white\_check\_mark: ~~[Cream-Browser](https://github.com/linkdd/cream-browser) ⭐ 9 | 🐛 2 | 🌐 C | 📅 2026-05-21~~ - A browser developped in C with GTK+ having the same interface as Vimperator.

* :white\_check\_mark: [qutebrowser](https://qutebrowser.org/)

* :white\_check\_mark: [Vieb](https://vieb.dev/) - Vim bindings for the web by design (electron-based)

* Firefox
  * :heavy\_plus\_sign: [Tridactyl](https://addons.mozilla.org/en-US/firefox/addon/tridactyl-vim/)
  * :heavy\_plus\_sign: [Vimium-FF](https://addons.mozilla.org/en-US/firefox/addon/vimium-ff/)
  * :heavy\_plus\_sign: [Vimium C](https://addons.mozilla.org/en-US/firefox/addon/vimium-c/)
  * :heavy\_plus\_sign: [Surfingkeys](https://addons.mozilla.org/en-US/firefox/addon/surfingkeys_ff/)
  * :heavy\_plus\_sign: [Vim Vixen](https://addons.mozilla.org/en-US/firefox/addon/vim-vixen/)
  * :heavy\_plus\_sign: [vimkeybindings](https://addons.mozilla.org/en-US/firefox/addon/vimkeybindings/) - Small addon adding just basic keyboard navigation shortcuts.
  * :heavy\_plus\_sign: [Krabby](https://krabby.netlify.app/) - keyboard-based navigation inspired by Kakoune.
  * :heavy\_plus\_sign: ~~[Vimperator](http://vimperator.org/vimperator)~~ - See Tridactyl instead
  * :heavy\_plus\_sign: ~~[Pentadactyl](https://en.wikipedia.org/wiki/Pentadactyl)~~ - See Tridactyl instead
  * :heavy\_plus\_sign: [Video Speed Controller](https://addons.mozilla.org/en-US/firefox/addon/videospeed/) – Allows remapping HTML5 video playback controls (e.g., seeking with `h/l`, speed adjustment with `j/k`) to match Vim-like navigation.

* Chrome
  * :heavy\_plus\_sign: ~~[cVim](https://github.com/1995eaton/chromium-vim) ⭐ 2,256 | 🐛 327 | 🌐 JavaScript | 📅 2022-10-19~~
  * :heavy\_plus\_sign: ~~[wasavi](https://github.com/akahuku/wasavi) ⭐ 1,543 | 🐛 130 | 🌐 JavaScript | 📅 2024-03-20~~ - Transform text areas into a vi editor.
  * :heavy\_plus\_sign: ~~[vrome](https://github.com/jinzhu/vrome) ⭐ 618 | 🐛 87 | 🌐 CoffeeScript | 📅 2016-10-24~~
  * :heavy\_plus\_sign: ~~[ViChrome](https://github.com/k2nr/ViChrome) ⭐ 229 | 🐛 29 | 🌐 CoffeeScript | 📅 2017-03-18~~
  * :heavy\_plus\_sign: [Vimium](https://chrome.google.com/webstore/detail/vimium/dbepggeogbaibhgnhhndojpepiihcmeb)
  * :heavy\_plus\_sign: [Vimium C](https://chrome.google.com/webstore/detail/vimium-c-all-by-keyboard/hfjbmagddngcpeloejdejnfgbamkjaeg?hl=en)
  * :heavy\_plus\_sign: [Surfingkeys](https://chrome.google.com/webstore/detail/surfingkeys/gfbliohnnapiefjpjlpjnehglfpaknnc)
  * :heavy\_plus\_sign: [Krabby](https://krabby.netlify.app/) - keyboard-based navigation inspired by Kakoune.
  * :heavy\_plus\_sign: [Video Speed Controller](https://chromewebstore.google.com/detail/video-speed-controller/nffaoalbilbmmfgbnbgppjihopabppdk) – Allows remapping HTML5 video playback controls (e.g., seeking with `h/l`, speed adjustment with `j/k`) to match Vim-like navigation.

* Safari
  * :heavy\_plus\_sign: [Surfingkeys](https://apps.apple.com/us/app/surfingkeys/id1609752330)
  * :heavy\_plus\_sign: [Vimari](https://apps.apple.com/us/app/vimari/id1480933944?ls=1\&mt=12) -  A Safari [extension](https://televator.net/vimari/) that provides Vim-style keyboard-based navigation, based on Vimium.

* Edge
  * :heavy\_plus\_sign: [Surfingkeys](https://microsoftedge.microsoft.com/addons/detail/surfingkeys/kgnghhfkloifoabeaobjkgagcecbnppg)

* Opera
  * :heavy\_plus\_sign: ~~[wasavi](https://github.com/akahuku/wasavi) ⭐ 1,543 | 🐛 130 | 🌐 JavaScript | 📅 2024-03-20~~ - Transform text areas into a vi editor.
  * :heavy\_plus\_sign: ~~[VimOperate](https://github.com/rscircus/VimOperate) ⭐ 9 | 🐛 4 | 🌐 JavaScript | 📅 2023-09-01~~

* :white\_check\_mark: [w3m](https://w3m.sourceforge.net/) - A text-based web browser with some Vim-like [keyboard shortcuts](https://cheatsheetfactory.geekyhacker.com/linux/w3m).

* :white\_check\_mark: [netrik](https://netrik.sourceforge.net/) - A text-based web browser with Vi-inspired keyboard commands.

* :white\_check\_mark: [lynx](https://lynx.invisible-island.net/) - A customizable text-based browser and the oldest web browser still being maintained. You can enable Vi-like movement by passing `-vikeys` or add an alias in your `.bashrc`:

  * ```bash
    alias lynx='lynx -vikeys'
    ```

* :white\_check\_mark: [vimb](https://fanglingsu.github.io/vimb/) - The vim like browser.

* :white\_check\_mark: [jumanji](https://pwmt.org/projects/jumanji) - A keyboard driven web browser.

* :white\_check\_mark: [luakit](https://luakit.github.io/) - A highly configurable browser with [Vim-like](https://wiki.archlinux.org/title/Luakit) navigation.

* :white\_check\_mark: [bombadillo](https://bombadillo.colorfield.space/) - A non-web browser but for other protocols, e.g., Gopher, Gemini, Finger.

* :white\_check\_mark: ~~[uzbl](https://www.uzbl.org/)~~

* Various
  * :heavy\_plus\_sign: [firenvim](https://github.com/glacambre/firenvim) ⭐ 6,108 | 🐛 95 | 🌐 TypeScript | 📅 2026-08-04 - Transform text areas into a Neovim instance that inherits your existing config (keymaps, plugins, etc).

## Window Managers

* :white\_check\_mark: [AppGrid](https://github.com/mjolnirapp/AppGrid) ⭐ 666 | 🐛 2 | 🌐 Objective-C | 📅 2026-06-14 - A window manager for macOS with Vim-like hotkeys.
* :white\_check\_mark: [howm](https://github.com/HarveyHunt/howm) ⭐ 657 | 🐛 17 | 🌐 C | 📅 2022-07-19 - A lightweight, X11 tiling window manager that behaves like vim.
* :white\_check\_mark: [howm](https://github.com/HarveyHunt/howm) ⭐ 657 | 🐛 17 | 🌐 C | 📅 2022-07-19 - A lightweight tiling X11 window manager that mimics vi.
* :white\_check\_mark: [wmii](https://github.com/0intro/wmii) ⭐ 137 | 🐛 0 | 🌐 C | 📅 2026-08-23 - A small and scriptable window manager that can be configured with Vim-like [keyboard shortcuts](https://wiki.debian.org/Wmii#Basic_Configuration).
* :white\_check\_mark: [i3wm](https://i3wm.org/) - A tilling window manager with Vim-like [keyboard shortcuts](https://i3wm.org/docs/refcard.html).
* :white\_check\_mark: [sway](https://swaywm.org/) - A drop-in replacement for i3 for Wayland.
* :white\_check\_mark: [euclid-wm](https://code.google.com/archive/p/euclid-wm/) - A minimalist tiling wm with default Vim-like keybindings.

## WYSIWYG Editors

* :white\_check\_mark: [zettlr](https://www.zettlr.com) - Markdown document editor on the fly, vim+emacs keybindings.
* :white\_check\_mark: [VNote](https://vnotex.github.io/vnote/en_us/) - A note taking app.

# Keyboard Remapping

Keyboard remapping tools can improve your efficiency while navigating across the system, as well as enhance your experience inside Vim.
They allow you to flexibly remap any key—for example, replacing the arrow keys with `hjkl`, among other useful remappings.\
Most of these tools are universal enough to work system-wide, even inside a Linux TTY, due to their low-level nature.

* :heavy\_plus\_sign: [keyd](https://github.com/rvaiya/keyd) ⭐ 5,922 | 🐛 318 | 🌐 C | 📅 2026-06-01 - A key remapping daemon for Linux.
  * <details>
      <summary>Example: Vim-like remaps using <code>keyd</code></summary>

    ```ini
    # A valid config file has the extension .conf and must begin with an [ids] section
    [ids]
    *

    [main]
    # Map Caps Lock to Escape when tapped and Control when held
    capslock = overload(control, esc) # Super useful for Vim and not only!

    # Make Alt a layer activator for the defined keys and act as regular Alt with all other keys
    [alt]
    h = left
    k = up
    j = down
    l = right

    0 = home
    4 = end
    # i = home
    # a = end

    u = pageup
    d = pagedown

    x = delete

    # Check the keyd repo for more!
    ```

    </details>

# Contributing

This is a collaborative list -- please fork and make a pull request to add or improve the entries here! The initial contributions by the repo owner are limited to the tools he uses or knows of, so there is a lot of room for further additions here!

* Please:
  * Add links to references for configuration if you have any.
  * Use [XDG paths](https://wiki.archlinux.org/title/XDG_Base_Directory) when possible.
* It's okay to list deprecated or unmaintained software for the sake of completeness, but let's put a ~~strikethrough~~ on them.

# Acknowledgments

Hats off to the authors of these articles that helped kick-start this list together with the author's own experiences: [#1](https://www.reddit.com/r/vim/comments/3tluqr/my_list_of_applications_with_vi_keybindings/), [#2](https://reversed.top/2016-08-13/big-list-of-vim-like-software/), [#3](https://www.slant.co/topics/7131/~programming-text-editors-with-vim-key-bindings), [#4](https://vim.reversed.top/), [#5](https://vim.fandom.com/wiki/Vim_key_bindings_for_web_browsers).

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._
