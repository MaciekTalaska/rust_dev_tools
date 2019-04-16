## Tooling for Rust developers

====

## Tig

- oquick, terminal based, git log capabilities
====

## Zeal
- sometimes you need documentation, but you're offline...
====

##  Tmux
- for developers who spend a lot of time in terminal, this is a must
- many windows / panels
- configuration could be saved (stored) on a machine, so it is easy to continue from the same state
====

## Source diffing tools + git config
- p4 merge / kompare / kdiff
- neither of ^^^ is perfect:

Notes:
  - p4mrerge can't handle diff of whole directory (git difftool -d)
  - kompare is pretty perfect, but its way of show differences on whitespaces is not the greatest
  - kdiff is all great, but the UI itself is pretty dated, and not that visually pleasing as kompare/p4merge
- git config is super important (for small changesets I actually used 'git diff')
- sometimes I also use xxdiff or vimdiff (but not so often)
====

## qgit 

- git again...
- visualize git tree

Notes:
- sometimes you really need to see a git tree in a visual way - but that doesn't mean installking some huge tool (Atlassian SourceTree etc) is a soliution
- alternatives (but much more bloat): atlassian SourceTree, GitKraken (free for personal use)
====


## asdf 
- idea of developing whole system in a single language is really nice, but not always possible
- asdf is multiplatform (Linux, OSX, and maybe WSL on Windows) version manager
- it allows to easy install, remove, change default version of particular programming language

====

## PatriciaSQL
-  small GUI application that simplifies querying PostgreSQL
- developed by myself in a free time, during couple of weeks end of 2018, beginning of 2019
- not 100% ready, but quite solid already and ready to use
====

## Nix + containers

- the best way to build small containers
- apart from ^^^ it is also great in managing developer related packages
(probably targeted at people using Linux/OSX)
====

## Virtual desktops
Notes: 
- I cant imaging working without many desktops, which I can easily switch between (and that needs to be availabla via shortcut)
- my setup is 4 virtual desktops, but I usually use not more than 3
- default setup is super important, for me it is:
  - #1 - konsole
  - #2 - web browser (if any) + zeal
  - #3 - editor(s) / IDE (usually Emacs or PyCharm/IndelliJ for Rust/Scala, VSCode for front-end development)
====

## IntelliJ / PyCharm + Rust Plugin
====

### Disadvantages:
- it is pretty big (but big is not objective, so lets count):
- IntelliJ is slow to start. Same as Emacs, VSCode, Atom...
- has VIM plugin, but still is not that convenient to use it without touching a mouse
- VIM plugin doesn't work that well with some default key binding, so some work is needed to make it work properly

Notes:
  - IntelliJ takes 500MB on disk, 160MB of that is Java. Config for IntelliJ grows over time ;( and may exceed 100 MB)
  - VSCode without plugins in 200 MB on disk. Plugins are adding a lot to that
  - Atom is pretty big: it used to be ~800 MB on disk, now it is only 500 MB (no plugins) but that is just an editor!
  - SublimeText3 is ~25 MB on disk
  - Vim grows a bit when using plugins. My VIM plugins are taking ~26 MB
  - Emacs: consumes ~250 MB but this is Emacs + lots of plugins (Clojure, Elixir, Erlang, Rust, Markdown, git, org-mode... )
====


### Advantages:
- IDE is not just a "bigger editor"
- refactoring is more than just changing variable name
- **proper** auto-complete
Why JetBrains tools? 
  - smart refactorings
  - type info
  - doc at hand
  - "suggestions" available
  - git/console integration

Notes:
- work in your editor of choice? is it based on understaning the code? or is it just "plain stupid?"
- I have been exposed to the JetBrains products when I first started working with their plugin for Visual Studio. And then I tried other tools they produced to find out they were also awesome. This is why:
      - which are super helpful not only to novice developers (the tool itself suggest possible ways code may be reorganized)
    - it helps you improving the code (unused imports, unused variables etc.)
====

### Free versions of JetBrains tools:
- PyCharm Community
- IntelliJ Community 
(whats the difference?)
====

### Rust plugin:
- some plugin features are available only with CLion (that has no community edition):
  - debugging
  - CPU profiler
====

### Rust plugin
- Rust is strongly typed language, and types are super  important (and are visible easily)
- Easy to search and navigate
- Goto/Find Usages
- Ctrl-Q for documentation
- Ctrl+Shift+P - get the type of expression selected
- Ctrl+J
- Ctrl+Alt+J

more info: https://intellij-rust.github.io/features/
