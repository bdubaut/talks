[.autoscale: true]
[.slide-transition: true]

# Debugging software with `git bisect`

---

[.slidenumbers: true]

```
git bisect start [--term-{new,bad}=<term> --term-{old,good}=<term>]
	  [--no-checkout] [--first-parent] [<bad> [<good>...]] [--] [<paths>...]
git bisect (bad|new|<term-new>) [<rev>]
git bisect (good|old|<term-old>) [<rev>...]
git bisect terms [--term-good | --term-bad]
git bisect skip [(<rev>|<range>)...]
git bisect reset [<commit>]
git bisect (visualize|view)
git bisect replay <logfile>
git bisect log
git bisect run <cmd>...
git bisect help
```

---

[.slidenumbers: true]

> `git bisect` uses a binary search algorithm to find which commit in your project’s history introduced a bug.

---

[.slidenumbers: true]

```bash
$> git bisect start
$> git bisect bad # Current version is bad
$> git bisect good # Current version is bad

```

---

[.slidenumbers: true]

Let's take it for a spin!
