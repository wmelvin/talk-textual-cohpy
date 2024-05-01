
# Building TUIs with Textual

---

## whoami

### Bill Melvin

- First programming language was BASIC
- Programming professionally since late 1980s
- Built systems using Pascal into late 2000s
    - Turbo Pascal
    - Borland Pascal
    - Delphi (Object Pascal)
- Back to BASIC in 2011 (VBA for automating MS-Access)
- Oldest of my own Python scripts I could find was written in 2006
- Started putting Python projects on GitHub in 2020

---

### More About Me

I am **not** an *Authority* or *Expert*

I **am** a *Learner*, *Explorer*, and *Experimenter*

I am **not** a *Computer Scientist* or *Software **E**ngineer*

However I **am** an experienced *Software Developer*

and I may have done some *software **e**ngineering*

(and perhaps a little *prompt **e**ngineering* as well ;)

<!-- 
I hesitate to call myself an "Engineer" because I do not have a college degree.
Nonetheless I have done work that would probably qualify as "software engineering."
-->

<!-- class: pg-more-about text-center -->

---

### At work in 1994

![Bill at work in 1994](images/Bill-at-DHI-Mar-94.jpg)

Probably working on a [Turbo/Borland Pascal](https://en.wikipedia.org/wiki/Turbo_Pascal) program, in a text-only interface, on a PC running [MS-DOS](https://en.wikipedia.org/wiki/MS-DOS).

I suppose in 1994, it could have been running [Windows 3.1](https://en.wikipedia.org/wiki/Windows_3.1), but I don't recall.

<!-- class: text-center img-70 -->

---

## Original Console / Terminal

- Commands: batch files, executable programs
- Programs with character-based UIs
- 80 x 25 character display
- **Limited interactivity**

![IBM PC](images/IBM_5154_-_PC_DOS_Prompt-crop-scale.jpg)

<!-- class: ibm-pc -->
---

## Graphical User Interface (GUI)

The [Graphical user interface](https://en.wikipedia.org/wiki/Graphical_user_interface) has largely replaced the earlier text-based UIs.

The term *Graphical User Interface* may have been used more in the past to make the distinction between this new style versus the text-based user interfaces common at the time GUIs were introduced more widely.

- Desktop applications

- Web browser / applications

- **Highly interactive**

---

### GUI - Python - Desktop

There are multiple options for creating GUIs in Python:

- Standard Library: [tkinter](https://docs.python.org/3/library/tk.html)
- [wxPython](https://wxpython.org/)
- [Qt for Python](https://doc.qt.io/qtforpython-6/)
- More: [Awesome Python - gui-development](https://github.com/vinta/awesome-python#gui-development)

<!-- class: dbl -->

---

### GUI - Python - Web

Web applications are also GUIs, and Python has many options for creating them:

- [Django](https://www.djangoproject.com/)
- [Flask](https://flask.palletsprojects.com/en/3.0.x/)
- [Quart](https://github.com/pallets/quart?tab=readme-ov-file#quart) (if you want async)
- [Pyramid](https://trypyramid.com/)
- [FastAPI](https://fastapi.tiangolo.com/) (not just APIs)
- More: [Awesome Python - web-frameworks](https://github.com/vinta/awesome-python#web-frameworks)

<!-- class: dbl -->

---

### GUI - Python - Web/Desktop

[PgAdmin4](https://www.pgadmin.org/) is an example of a web application that can run locally or on a server.

![PgAdmin4 screen](images/screen-pgAdmin4.jpg)

> "pgAdmin 4 is a complete rewrite of pgAdmin, built using Python and Javascript/jQuery. A desktop runtime written in NWjs allows it to run standalone for individual users, or the web application code may be deployed directly on a web server for use by one or more users through their web browser."

<!-- class: text-center img-70 -->
---

## Do you need a GUI?

If you're building a web, or mobile, application, the answer is **yes** (by default).

If you're building a utility that will run on a local machine, the answer is **it depends**.

- If the output is essentially graphical in nature (data visualization, etc.), you probably do want a GUI.
- Otherwise you may want to consider a simpler option.

<!-- class: dbl -->

---

## Inputs to Python apps

### CLI

#### Command-line arguments

- sys.argv
- Argparse
- Click

#### Promps:

- Input()
- Click `prompt=`

---

### Python - input

![Python input](images/code-py-input-1.png)

![Python output](images/code-py-input-2.png)

<!-- class: img-50 -->

---

## TUI - Textual User Interface

### Something in-between a CLI and a GUI

- More dynamic than CLI options and prompts.

### Why would you want to build a TUI?

- You like doing things in the console/terminal.

- Your application could use more than command line input, but doesn't warrant a full desktop or web GUI.

---

## Textual

### How I heard about Textual

#### Podcast - Talk Python to Me

[Talk Python to Me](https://talkpython.fm/)

![Talk Python to Me logo](images/podcast-talkpython.jpg)

[Episode #336](https://talkpython.fm/episodes/show/336/terminal-magic-with-rich-and-textual) - Terminal magic with Rich and Textual

[Episode #380](https://talkpython.fm/episodes/show/380/7-lessons-from-building-a-modern-tui-framework) - 7 lessons from building a modern TUI framework

<!-- class: img-auto -->

---

#### Podcast - Python Bytes

[Python Bytes](https://pythonbytes.fm/)

![Python Bytes logo](images/podcast-pythonbytes.jpg)

[Episode #299](https://pythonbytes.fm/episodes/show/299/will-mcgugan-drops-by) - Will McGugan drops by

<!-- class: img-auto -->

---

#### Podcast - Real Python Podcast

[Real Python Podcast](https://realpython.com/podcasts/rpp/)

![Real Python Podcast logo](images/podcast-realpython.jpg)

[Episode #80](https://realpython.com/podcasts/rpp/80/) - Make Your Python App Interactive With a Text User Interface (TUI)

Article: [Python Community Interview With Will McGugan](https://realpython.com/interview-will-mcgugan/)

<!-- class: img-auto -->

---

### Will McGugan

[github.com/willmcgugan](https://github.com/willmcgugan)

![Will McGugan GitHub](images/github-WillMcGugan.jpg)

<!-- class: text-center -->

---

#### Will McGugan - Textualize/Rich

[Textualize/rich](https://github.com/Textualize/rich#readme)

> "Rich is a Python library for rich text and beautiful formatting in the terminal."

![Rich screenshot](images/screen-rich.jpg)

<!-- class: text-center -->

---

## Textualize/Textual

[textual.textualize.io](https://textual.textualize.io/)

![Textual Welcome Screen](images/textual-welcome.jpg)

<!-- class: text-center -->

---

### Textual App Examples


[bloomberg/memray](https://github.com/bloomberg/memray#readme): Memray is a memory profiler for Python

[Textualize/frogmouth](https://github.com/textualize/frogmouth): A Markdown browser for your terminal

---

### Tutorial

[Tutorial](https://textual.textualize.io/tutorial/)

- Stopwatch app

---

### Aspects of Textual

- [Widgets](https://textual.textualize.io/widget_gallery/)

- [Composition](https://textual.textualize.io/guide/app/#composing)

- [Events](https://textual.textualize.io/guide/app/#events)

- [Reactivity](https://textual.textualize.io/guide/reactivity/)

- Class and Id: [DOM Queries](https://textual.textualize.io/guide/queries/)

- TCSS: [Textual CSS](https://textual.textualize.io/guide/CSS/)

---

## My Application

### A Pomodoro Timer

---

### Pomodoro Technique

![Wikipedia Pomodoro Technique](images/wikipedia-pomodoro-technique.png)

[Pomodoro Technique](https://en.wikipedia.org/wiki/Pomodoro_Technique)


<!-- class: text-center -->

---

#### Pomodoro Timer - Classic

Tick, tick, tick... RING!

![Pomodoro Timer](images/timer-pomororo-2-600.jpg)

<!-- class: timer-pic -->

---

#### Pomodoro Timer - Home Office

This one beeps when it's done, but doesn't tick the whole time.

![Digital Kitchen Timer](images/timer-digital-1-600.jpg)

<!-- class: timer-pic -->

---

#### Pomodoro Timer - Cubicle Land

It can be set to blink quietly.

![Digital Timer Blinks](images/timer-digital-2b-600.jpg)

<!-- class: timer-pic -->

---

#### Pomodoro Timer - Not!

![Rana Timer](images/timer-rana-600.jpg)

Well, it can be, if you want.

<!-- class: timer-pic -->

---

#### Spreadsheet

- I have been using a spreadsheet to track pomodoro sessions.
- It's not a timesheet - I don't track all work.
- I have other things on other tabs, so I want to keep using the spreadsheet.

![Pomodori Spreadsheet](images/pomodori-spreadsheet.png)

<!-- class: pg-spreadsheet -->

---

## Git

I use [git](https://git-scm.com/) for source code management.

Some projects are on [GitHub](https://github.com/wmelvin). Others are pushed to a local git server.

Some projects, such as one-off utility scripts, are not in git at all, but are backed up locally (and off-site).

---

## pipx

> "pipx is made specifically for application installation, as it adds isolation yet still makes the apps available in your shell: pipx creates an isolated environment for each application and its associated packages."

I have been using [pipx](https://github.com/pypa/pipx#readme) to install Python command-line applications (not libraries).

<!-- class: dbl -->

---

### pipx - Install Python Applications

I use **pipx** to install some Python tools.

`pipx install hatch`

`pipx install pgadmin4`

I also like to install my own tools, outside of development, using pipx.

`pipx install pomodorable`

Packages don't have to be on PyPI, but you have to **specify the path** to a `.whl` file. One uploaded to a GitHub release will work.

`pipx install image_snip@https://github.com/wmelvin/image-snip/releases/download/v2024.03.1/image_snip-2024.3.1-py3-none-any.whl`

 A `.whl` file uploaded to a web hosting platform will also work.

`pipx install gitramble@https://bogusoft.com/packages/gitramble/gitramble-0.1.dev1-py3-none-any.whl`

---

## Project tools

- [Hatch](https://hatch.pypa.io/latest/) - Python project manager (environments, packaging, and more)
- [Ruff](https://docs.astral.sh/ruff/) - linter and code formatter (integrated with Hatch)
- [pytest](https://docs.pytest.org/en/stable/) - testing framework
- [Just](https://github.com/casey/just#readme) - command runner

<!-- class: dbl -->

---

### ruff

- **Linter** and **Formatter**
- configure in pyproject.toml (or ruff.toml)
- Hatch integrates Ruff

<!-- class: dbl -->

---

### Just

[just a command runner](https://github.com/casey/just#readme)

> "`just` is a handy way to save and run project-specific commands.
> Commands, called recipes, are stored in a file called `justfile` with syntax inspired by `make`..."

I learned about `just` looking at some of Simon Willison's projects on GitHub. I saw a file named `Justfile` and wondered what it does.

<!-- class: pg-just -->

---

#### Simon Willison

- [github.com/simonw](https://github.com/simonw)
- Post: [just-with-django.md](https://github.com/simonw/til/blob/f57ab1cddaee30af59c063ab857dac15f6d62376/django/just-with-django.md#L15)
- Post: [Python packages with pyproject.toml and nothing else](https://til.simonwillison.net/python/pyproject)

![Simon Willison GitHub](images/github-SimonWillison.jpg)

---

## Textual Development Tools

- Textual [Devtools](https://textual.textualize.io/guide/devtools/)
- [tcss-vscode-extension](https://github.com/Textualize/tcss-vscode-extension#readme): VS Code extension that enables syntax highlighting for Textual CSS files.
- [pytest-textual-snapshot](https://github.com/Textualize/pytest-textual-snapshot#readme): Snapshot testing for Textual applications

<!-- class: dbl -->

---

## Showstoppers?

When planning a project, it is good to think about potential showstoppers.

- Is what you want the project to do actually possible.

- Are there capabilities needed for the application to succeed that are not available in the language, framework, or platform?

<!-- class: dbl -->

---

### A Toasty Requirement

For a *Pomodoro Timer* application to be useful, it needs to **notify** you when the countdown is finished.

It was encouraging to see that Textual has a [Toast](https://textual.textualize.io/widgets/toast/) widget. Unfortunately, Textual's Toast widget only pops up in the terminal. I want a **system notification**.

Searching for a Python package to do system notifications turned up a few. Some were Windows-only. Some required installing additional system packages.

I settled on **plyer**:

- part of the [Kivy](https://kivy.org/) project
- does notifications on multiple platforms

---

### Small POC to verify

Python script **toasty**

Ran on:
- Multiple Linux PCs and VMs (Debian - based)
- Windows 10 PC
- Windows 11 VM on Azure (I have no PCs that Microsoft considers worthy of running Windows 11 - oh well)
- I have no Mac, so not tested on that OS

<!-- class: dbl -->

---

## Project Setup

### hatch init

Running `hatch init` creates scaffolding for a Python project.

- Directory tree (uses a [src layout](https://packaging.python.org/en/latest/discussions/src-layout-vs-flat-layout/))
- Default `LICENSE` and `README` files
- [pyproject.toml](https://packaging.python.org/en/latest/specifications/pyproject-toml/)


I made some edits before doing the initial `git commit`.


---

## Project Dependencies

### Packages used

- [Textual](https://textual.textualize.io/) - Textual User Interface framework
- [Click](https://palletsprojects.com/p/click/) - command-line options
- [platformdirs](https://github.com/platformdirs/platformdirs#readme) - common directories on different platforms
- [plyer](https://pypi.org/project/plyer/) - system notifications
- [python-dotenv](https://pypi.org/project/python-dotenv/) - override default settings during development
- [tomlkit](https://pypi.org/project/tomlkit/) - store configuration as TOML

---

## Application

### Classes

#### AppConfig

#### AppData

- config
- file output
- cli_functions

#### UI(App)

---

### Textual - Bindings

[Bindings](https://textual.textualize.io/guide/input/#bindings) are declared in the App class.

![BINDINGS](images/code-textual-bindings-1.png)

Actions are implemented with the method name starting with `action_` followed by the action defined in the `BINDINGS` list.

![Actions](images/code-textual-bindings-2.png)

The action descriptions show in the app's Footer.

![Footer](images/app-footer.png)

<!-- class: img-50 -->

---

#### Click for CLI

- Some options are CLI-only

- Otherwise run the UI

---

## Testing a Textual App

Textual Guide: [Testing](https://textual.textualize.io/guide/testing/)

Snapshot testing for Textual apps: [pytest-textual-snapshot](https://pypi.org/project/pytest-textual-snapshot/)

<!-- class: dbl -->

---

## Using the App

### Outputs

**Data CSV** - Stored in user app data location.

**Daily CSV** - Aligns with the layout of the spreadsheet I've been using for years.

**Daily Markdown** - Written to an [Obsidian](https://obsidian.md/) *Daily Notes* file.

---

### Showstoppers? - Part II

#### Segfault

![Segfault](images/screen-segfault.jpg)


- Not sure why this happened, but I suspect I was misusing the timer event and reactivity.

- By default Ubuntu does not write core-dump files for user packages, so there was not one to look at (as if I'd know what I was looking at ;)


---

## What Else?

Some commits to look at (maybe):

- Initial UI mockup phase
- Adding the TimerBar that mimics the markings on the classic timer.

Some aspects to look at in the code:

- Using classes to manage app state.
- Using `textual run --dev` to see TCSS changes live.

*Gotchas*

- Events, reactivity, and watchers
- TCSS default styles on widgets (ex. Button min-width 16)
- When to use async

---

## What's Next?

### Possible Enhancements

Here are a few things I may (or may not) do with the Pomodorable app:

- Add documentation using [Material](https://squidfunk.github.io/mkdocs-material/) for [MkDocs](https://www.mkdocs.org/).

- Add a function to play a sound when a session is finished - maybe the sound of the classic kitchen timer ringing.

- Create an alternate `AppData` class that talks to a web API instead of the file system. That would require a web back-end, perhaps built using [FastAPI](https://fastapi.tiangolo.com/).

---

## That's All

### Thank you

[wmelvin.dev](https://wmelvin.dev/)

___

You can find more of my ramblings in my "[stuff](https://github.com/wmelvin/stuff)" repo on GitHub.

<!-- class: the-end text-center -->
