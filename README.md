# kayfabe

A fake terminal that makes your computer look busy. It types commands, runs
builds, fails tests, fixes them, and fills the screen with dashboards, charts
and logs, none of it real.

![ops dashboard](screenshots/dashboard.png)

| | |
|---|---|
| ![release](screenshots/release.png) | ![metrics](screenshots/areachart.png) |

## Run it

```
./kayfabe            # Ctrl+C to quit
./kayfabe --speed 2  # twice as fast; 0.5 is slower
```

One Python file, standard library only, Python 3.8+. Copy it to any Mac and run it.

## What you'll see

Git pulls and pushes, npm/pip/cargo/go builds, pytest and jest runs (with
failures that get fixed in vim and re-run), docker builds and pulls, kubectl,
terraform, ssh sessions, flame graphs, request traces, a live ops dashboard,
area charts, a network traffic view, matrix rain, and a gradient banner when a
"release" ships. Everything is randomized, and the mix changes with the
project it is pretending to work on.

Every few commands it stops at a prompt (deploy? password? host key?). If you
type something it accepts it; if you don't, it waits a few seconds and answers
for itself.

## It's harmless

It only prints text. It makes no network calls, runs no subprocesses, reads and
writes no files, and sends no keystrokes to the OS. Anything you type at one of
its prompts is thrown away. The only thing it reads from the machine is your
username, hostname and macOS version, for realism. Hostnames, domains, AWS
accounts and companies in the output are invented.

## License

MIT
