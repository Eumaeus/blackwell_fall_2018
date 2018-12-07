# Greek Workflow Overview

## Starting the Virtual Machine

1. In a terminal (`Terminal.app` on MacOS, `Git-Bash` on Windows), move into `fall2018vm` using `cd`:  `cd ~/Desktop/fall2018vm`.
1. `vagrant up` starts the virtual machine.
1. `vagrant ssh` connects your Terminal session to the virtual machine.
1. `cd /vagrant/ez-morph` to navigate to the morphology tools.
1. `git pull` to get any updates to the scripts and data.
1. `sbt console` to start the programming environment.

## MS Word View

In `sbt console` (you should see a `scala` prompt)…

1. `:reset`
1. `:load tools.sc` 
1. `analyzeFile("unit4")`

The resulting file, `unit4.docx` will be on your (host) computer at `~/Desktop/fall2018fm/ez-morph/documents/unit4.docx`.

You an do `analyzeFile()` on `"unit4a"`… `"unit4e"` to work in smaller chunks. Open the corresponding `.docx` file, *e.g.*, `unit4a.docx`.

## Web View

In `sbt console` (you should see a `scala` prompt)…

1. `:reset`
1. `:load webify.sc` 
1. `analyzeFile("unit4")` 

**In the Host Computer's fileystem** go to `~/Desktop/fall2018vm/ez-morph/documents`. Open `unit4.html` in a browser.

## When Done

1. `:quit`
1. `logout`
1. `vagrant halt`

