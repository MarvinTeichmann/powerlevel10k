## powerlevel9k Theme for Oh-My-Zsh

This is a theme for [Oh-My-Zsh](https://github.com/robbyrussell/oh-my-zsh). This
theme uses [Powerline Fonts](https://github.com/Lokaltog/powerline-fonts), thus
giving you the most epic terminal styling in the universe (as of 2015 C.E.).

Look like a bad-ass. Impress everyone in 'Screenshot Your Desktop' threads. Use powerlevel9k.

In addition to looking amazing, this theme actually provides a lot of useful
information.

### Features

* Mercurial support is now in development Check out the `mercurial_support` branch!

* Shows lots of information about Git repositories, including:
    * branch / tag name
    * current action status (rebasing, merging, etc.,)
    * being behind / ahead of your remote
    * various local working tree statuses
* Shows command number in right-prompt (so you can `$ !<num>` to re-run)
* Shows return-code of command if it is an error code
* Shows system time in right-prompt
* Indicates background jobs with a gear
* Will conditionally display the `user@host` string

**If you would like an OMZ theme that provides most of the same features but
doesn't require Powerline fonts, check out the sister font,
[hackersaurus](https://github.com/bhilburn/hackersaurus).**

These screenshots should give you an idea of what `powerlevel9k` looks like:

![](http://bhilburn.org/content/images/2014/12/powerlevel9k.png)

![](http://bhilburn.org/content/images/2015/01/pl9k-improved.png)


### Installation

First, you need to install Powerline Fonts. You can find the [installation
instructions
here](https://powerline.readthedocs.org/en/latest/installation/linux.html#fonts-installation).
You can also find the raw font files [in this Github
repository](https://github.com/powerline/fonts).

To install this theme, drop the `.zsh-theme` file into your `.oh-my-zsh/custom/themes`
directory:

    $ cd ~/.oh-my-zsh/custom/themes
    $ git clone https://github.com/bhilburn/powerlevel9k.git powerlevel9k

You then need to select it in your `~/.zshrc`:

    ZSH_THEME="powerlevel9k/powerlevel9k"

If you do not want to display the `user@host` string, you should also put this
in your `~/.zshrc`:

    export DEFAULT_USER=<your username>

### Customization

You can choose which segments are shown on each side. Just add the following variables to
your `~/.zshrc`. The below also shows the default settings if you don't define
your own.

    POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(context dir git)
    POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(status history time)

### Bugs / Contact

If you have any requests or bug reports, please use the tracker in this Github
repository.
