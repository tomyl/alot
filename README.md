[![Build Status][travis-img]][travis]
[![Code Climate][codeclimate-img]][codeclimate]
[![Codacy Grade][codacy-grade-img]][codacy-grade]
[![Codacy Coverage][codacy-coverage-img]][codacy-coverage]


Alot is a terminal-based mail user agent based on the [notmuch mail indexer][notmuch].
It is written in python using the [urwid][urwid] toolkit and features a modular and command prompt driven interface to provide a full MUA experience as an alternative to the Emacs mode shipped with notmuch.


Notable Features
----------------
 * multiple accounts for sending mails via sendmail
 * can spawn terminal windows for asynchronous editing of mails
 * tab completion and usage help for all commands
 * contacts completion using customizable lookups commands
 * user configurable keyboard maps
 * customizable colour and layout themes
 * python hooks to react on events and do custom formatting
 * forward/reply/group-reply of emails
 * printing/piping of mails and threads
 * configurable status bar with notification popups
 * database manager that manages a write queue to the notmuch index
 * full support for PGP/MIME encryption and signing


Installation and Customization
------------------------------
Have a look at the [user manual][docs] for installation notes, advanced usage,
customization, hacking guides and [frequently asked questions][FAQ].
We also collect user-contributed hooks and hacks in a [wiki][wiki].

Most of the developers hang out in `#alot@freenode`, feel free to ask questions or make suggestions there.
You are welcome to open issues or pull-requests on the github page.


Basic Usage
-----------
The arrow keys, `page-up/down`, `j`, `k` and `Space` can be used to move the focus.
`Escape` cancels prompts and `Enter` selects. Hit `:` at any time and type in commands
to the prompt.

The interface shows one buffer at a time, you can use `Tab` and `Shift-Tab` to switch
between them, close the current buffer with `d` and list them all with `;`.

The buffer type or *mode* (displayed at the bottom left) determines which prompt commands
are available. Usage information on any command can be listed by typing `help YOURCOMMAND`
to the prompt; The key bindings for the current mode are listed upon pressing `?`.
See the [manual][docs] for more usage info.



[notmuch]: http://notmuchmail.org/
[urwid]: http://excess.org/urwid/
[docs]: http://alot.rtfd.org
[wiki]: https://github.com/pazz/alot/wiki
[FAQ]: http://alot.readthedocs.io/en/latest/faq.html
[features]: https://github.com/pazz/alot/issues?labels=feature

[travis]: https://travis-ci.org/pazz/alot
[travis-img]: https://travis-ci.org/pazz/alot.svg?branch=master
[codacy-coverage]: https://www.codacy.com/app/patricktotzke/alot?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pazz/alot&amp;utm_campaign=Badge_Coverage
[codacy-coverage-img]: https://api.codacy.com/project/badge/Coverage/fa7c4a567cd546568a12e88c57f9dbd6
[codacy-grade]: https://www.codacy.com/app/patricktotzke/alot?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=pazz/alot&amp;utm_campaign=Badge_Grade
[codacy-grade-img]: https://api.codacy.com/project/badge/Grade/fa7c4a567cd546568a12e88c57f9dbd6
[codeclimate-img]: https://codeclimate.com/github/pazz/alot/badges/gpa.svg
[codeclimate]: https://codeclimate.com/github/pazz/alot
