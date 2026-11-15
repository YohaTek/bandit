# bandit

My working notes and solutions for [OverTheWire Bandit](https://overthewire.org/wargames/bandit/),
a beginner wargame for learning the Linux command line.

Each level gets one short note: what the level asks for, the command that
solves it, and the reasoning behind it. The goal is a walkthrough I can reread
later, not a spoiler dump — the point is understanding the shell, not copying
answers.

## Layout

```
levels/level-00.md   connection details and the first login
levels/level-01.md   (next)
...
```

One file per level, numbered to match the wargame. Files are added as I work
through the levels.

## Before you start

- An SSH client (`ssh`, present on any Linux or macOS machine).
- `proxychains` if your network blocks outbound SSH:
  `sudo apt install proxychains4`.
- Comfort with a terminal. No prior Linux knowledge is assumed — that is the
  whole point of the wargame.

## Connecting

The notes in `levels/` use a private instance of the game:

```sh
ssh bandit0@13.63.65.121 -p 2220
```

If that host is unreachable, use the public OverTheWire instance instead, which
listens on port `2220` as well:

```sh
ssh bandit0@bandit.labs.overthewire.org -p 2220
```

When SSH egress is blocked, prefix the command with `proxychains` as shown in
the level notes.

Passwords are not committed to this repository; they are stored outside the
working tree, and `.gitignore` covers common scratch filenames.

## Progress

| Level | Notes |
| ----- | ----- |
| 0 | [levels/level-00.md](levels/level-00.md) |
| 1–33 | not yet written |

## License

No license file yet. Content is personal study notes; open an issue if you want
to reuse it and we can sort out terms.
