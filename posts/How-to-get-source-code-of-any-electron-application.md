---
title: How to get source code of any electron application
date: 2017-12-06
tags:
  - electron
---

So there is a way to get source code of a closed source electron app. Generally all the electron apps are packed through asar and you can unpack the same using this module. For an example, if you want to see the source code of Slack app then you need to do following things -

    # **Open terminal and install asar node module globally**

    $ npm install -g asar

    # **Go into the app’s directory, in our case it’s Slack**

    $ cd /Applications/Slack.app/Contents/Resources

    # **Create a directory to paste the content of app**

    $ mkdir example-sourcecode

    # **Unpack the app.asar file in the above directory using asar**

    $ asar extract app.asar example-sourcecode

    # **Boom cd into it and see the source code of the app**

(**Note **— This post was originally posted here — [https://howtoelectron.app/](https://howtoelectron.app/))
