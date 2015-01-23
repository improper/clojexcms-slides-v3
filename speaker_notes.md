# Preparation

* DB, LT
* fix browser-repl port
* start server
* prepare Chrome
* close other apps
* turn off Wifi

***

# Welcome

* my first talk since university
* glad to be here

# My background

* Web development since 2001
* Perl, Ruby on Rails
* finally happy (for now) with Clojure(Script)

# Slide: Outline

# Slide: Motivation

* lots of information about single parts and libs
* show the big picture, how does it all come together?

## Use case

* Website with frontend and backend, simple CMS
* Frontend rendered server-side for search engines
* Content snippets displayed in the frontend can be edited

# Live Demo: Show the CMS

* conflicting edits warning: better than nothing but not a good UX

# Slide: Architecture

* Chestnut template
* no ORM, just plain SQL for migrations and runtime

# Slide: LOC

# Live Demo: Light Table

* nice environment, powerful out of the box
* plug-in mechanism, but nothing essential (yet)

## Server-side

* tear down JVM
* show workspace, connections, console
* start server again
* show database and SQL files
* show content-page and backend
* live-eval database query, show docs for function

## Client-side

* show core, state and server
* show frame and views/content
* live-eval in state: (-> js/document .-body (.setAttribute "style" "background: cyan"))
* live-eval in state: (swap! app-state update-in [:site :name] ":clojureD")
* set watch in content, l. 18, then type in browser
* show external browser, port needs to be set in env/dev/clj/clojexcms/dev.clj

# Slide: Conclusion

* LT issues: large files, Yosemite

# Slide: Thank you!

***

# Light Table Features and Issues

* Evaluation
* Docs (^D)
* Watches
* internal vs. external browser, port needs to be set, will be default in the future
* large CSS: impossible!
* Codemirror vim mode sucks
* Problems under Yosemite, will switch to Atom
