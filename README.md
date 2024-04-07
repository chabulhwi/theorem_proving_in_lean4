Theorem Proving in Lean 4
-----------------------

This is a fork of ["Theorem Proving in Lean 4"](https://github.com/leanprover/theorem_proving_in_lean4)
by Jeremy Avigad, Leonardo de Moura, Soonho Kong and Sebastian Ullrich, with contributions from the Lean
Community.

Note that *none* of the changes I made to the original text was endorsed by the original authors.

### Major Changes in My Fork

commit 50104743de63ed2f0554ab63ae0792ae46b5b189
Author: Bulhwi Cha <chabulhwi@semmalgil.com>
Date:   Sun Apr 7 20:04:34 2024 +0900

    doc: add cautionary note for constructivists

    This note may help constructivists thinking of using Lean to save time.

commit c002809407f9e82870a72d18886ec36dbffc893c
Author: Bulhwi Cha <chabulhwi@semmalgil.com>
Date:   Sun Apr 7 13:35:15 2024 +0900

    doc: clarify how Lean supports constructive logic

    The paragraph I added explains how Lean core [supports constructive
    logic][classical-tactics], whether the Lean core team will provide
    tactics for constructive logic or [accept them from
    contributors][not-priority], and whether a user can [develop them by
    oneself][not-stopping] [outside the core][possible].

    [classical-tactics]: https://leanprover.zulipchat.com/#narrow/stream/348111-std4/topic/Movement.20from.20Std.20to.20Init/near/430339840
    [not-priority]: https://leanprover.zulipchat.com/#narrow/stream/348111-std4/topic/How.20classical.20is.20std4.3F/near/383780177
    [not-stopping]: https://leanprover.zulipchat.com/#narrow/stream/270676-lean4/topic/constructive.20tactic.20mode.20in.20lean/near/431685357
    [possible]: https://leanprover.zulipchat.com/#narrow/stream/270676-lean4/topic/constructive.20tactic.20mode.20in.20lean/near/431714863

    Co-authored-by: Mario Carneiro <di.gama@gmail.com>
    Co-authored-by: Henrik Böving <hargonix@gmail.com>
    Co-authored-by: Scott Morrison <scott.morrison@gmail.com>

---

This manual is generated by [mdBook](https://github.com/rust-lang/mdBook). We are currently using a
[fork](https://github.com/leanprover/mdBook) of it for the following additional features:

* Add support for hiding lines in other languages [#1339](https://github.com/rust-lang/mdBook/pull/1339)
* Replace calling `rustdoc --test` from `mdbook test` with `./test`

To build this manual, first install the fork via
```bash
cargo install --git https://github.com/leanprover/mdBook mdbook
```
Then use e.g. [`mdbook watch`](https://rust-lang.github.io/mdBook/cli/watch.html) in the root folder:
```bash
mdbook watch --open  # opens the output in `out/` in your default browser
```

Run `mdbook test` to test all `lean` code blocks.

## How to deploy

```
./deploy.sh
```
