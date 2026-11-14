# Folkway, More, or Taboo?

An interactive card sort about norms. Students sort 16 behaviors as folkways, mores, or taboos, get a short explanation after each, and end with their full sort to compare with classmates. Some cards are clear-cut; others are borderline, depend on the culture, or have changed over time. By Gwen Sharp, as a companion to the norms material in *A Sociology Experiment* (Chapters 3 and 5).

**Live site:** https://gsharpokie.github.io/normsort/

## What it does

- **Three definitions** stay at the top of the page.
- **One card at a time.** After each choice, the page shows a label (Clear-cut, Borderline, Depends on place, or Changed over time), the usual answer, and a sentence or two of explanation. Borderline cards accept more than one answer.
- **Your sort:** every card under the category the student chose, with the usual answer noted where it differs.
- **What the hard ones show,** plus discussion questions (including one that asks students to write their own card).

Nothing a student selects is saved or sent anywhere.

## For instructors

- It works well in pairs: students sort separately, then compare their final lists.
- To show the full list without sorting, add `#list` to the link: https://gsharpokie.github.io/normsort/#list
- The “usual answers” are a starting point for discussion, not measured facts.

## Editing the cards

Open `index.html` on GitHub, select the pencil icon, and find `const CARDS = [` near the top of the `<script>` section. Each card looks like this:

```js
{ t: "Cutting into the middle of a long line", ok: ["folk", "more"], kind: "border",
  note: "It’s usually taught as a folkway, but watch how people react…" },
```

- `t` is the behavior. `note` is the explanation shown after the student chooses.
- `ok` lists the answer or answers that count as matching: `"folk"`, `"more"`, `"taboo"`.
- `kind` is the label: `"clear"`, `"border"` (borderline), `"place"` (depends on place), or `"time"` (changed over time).
- Use curly quotes and apostrophes, and keep the comma after each card’s closing brace except the last.
- If you change the number of cards, also change “16” in the page’s introduction and description.

## Turning on the site (one time)

Go to **Settings → Pages**. Under **Build and deployment**, set **Source** to **Deploy from a branch**, choose the **main** branch and the **/ (root)** folder, and select **Save**. Keep Issues turned on so the “Suggest one” link works.

## Sources

Sumner, William Graham. 1906. *Folkways*. Ginn. Douglas, Mary. 1966. *Purity and Danger*. Routledge. Haidt, Jonathan. 2001. “The Emotional Dog and Its Rational Tail.” *Psychological Review* 108(4): 814–834.

## Author

Created by Gwen Sharp ([@gsharpokie](https://x.com/gsharpokie)).

## License

© 2026 Gwen Sharp. Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): you may share and adapt it for noncommercial purposes with credit. See [LICENSE](LICENSE).
