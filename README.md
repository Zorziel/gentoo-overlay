# QOwnNotes Gentoo Overlay

This is a Gentoo overlay for [QOwnNotes](http://www.qownnotes.org), the open source (GPL) plain-text file notepad with markdown support and todo list manager for GNU/Linux, Mac OS X and Windows, that (optionally) works together with the notes application of Nextcloud/ownCloud.

## Usage

Add the QOwnNotes repository with the following command.

```bash
eselect repository enable qownnotes-overlay
```

Then you can install QOwnNotes the usual way.

```bash
emerge --sync qownnotes-overlay && emerge -av qownnotes
```

If you run into troubles with libpcre you might have to do a `env USE=pcre16 emerge -1 libpcre`.
