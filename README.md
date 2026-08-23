## Hi, I'm Nissan

I build small tools that show you what your computer is quietly telling
everyone else.

I got here from the other direction. Working out how to get into systems is
what taught me where they leak, and most of what I have published is that
knowledge pointed back the other way: here is what you are giving away,
here is why it matters, and here is what you can actually do about it.

### The tools

Each one reads something you already have, explains what it gives away, and
changes nothing.

| | Reads | Tells you |
|---|---|---|
| **[Glasshouse](https://github.com/NissanBoss/Glasshouse)** | your machine | what it says about you, sorted by how much of it you can actually change |
| **[Baggage](https://github.com/NissanBoss/Baggage)** | a file, before you send it | text buried under black boxes in PDFs, GPS in photos, tracked changes in Word |
| **[Alibi](https://github.com/NissanBoss/Alibi)** | your git history | forgotten addresses, your timezone, the hours you sleep, the identities it ties together |
| **[Haunts](https://github.com/NissanBoss/Haunts)** | the wireless networks your computer remembers | the places those names say you have been |

And two that are not audits:

| | |
|---|---|
| **[Octavo](https://github.com/NissanBoss/Octavo)** | turns a PDF into a booklet you can print at home, fold and staple. No LaTeX, no upload |
| **[Fal](https://github.com/NissanBoss/Fal)** | a programming language in Spanish, with no strange symbols in it |

### The rules they all follow

**They only read.** Nothing writes to what it was pointed at. Where that
matters most, a test hands the program the same path for input and output
and checks the file is untouched afterwards.

**Nothing goes anywhere.** No uploads, no lookups, no telemetry. Not as a
promise: there is no network code in any of them, and a test reads the
source and fails the build if any appears.

**No dependencies.** Not a small number. None. That includes writing a
Deflate decompressor by hand for the one built in Rust, because Rust's
standard library has no zlib in it.

**A gap is not a pass.** When something cannot be read, it says so, in its
own section, before any of the findings. A short report is not a clean
machine, and a tool that quietly gives up is worse than no tool: it hands
you confidence you have not earned.

**Everything is masked by default.** A report you paste into a chat should
not be the thing you were trying to keep. `--reveal` when you mean it.

### Elsewhere

Spain. Go mostly, and Rust when it earns its place.
