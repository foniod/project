Guide to new contributors
=========================

Thanks for contributing to `ingraind` and RedBPF!

Before getting into the best way to participate in the project, please
take a look at our [code of conduct](./CODE_OF_CONDUCT.md).

## Have a question?

If you have a question about using
[ingraind](https://github.com/ingraind/ingraind) or
[RedBPF](https://github.com/ingraind/redbpf), please raise a ticket in
the respective repository, or visit our [Matrix
channel](https://app.element.io/#/room/!vCJcBZDeGUXaqSvPpL:rustch.at?via=rustch.at).

## Would like to contribute something?

If you have an exact requirement with a solution, and `ingraind` or
RedBPF do not support it yet, feel free to open a PR.

We aim to maintain a high quality of contributions, and therefore all
PRs need to go through a review process. During the review period you may be
asked to make changes to the code.

In case you are not certain that your code quality or the feature
you're implementing is suitable for the project, please open an issue
with the question, or send the PR anyway. This allows the maintainers
to give you hands on feedback, and highlight anything you may not have
considered.

A quick checklist of things a PR should have:

 * All public API items need to have documentation.
 * Don't break public APIs unnecessarily.
 * Adding new API items is generally fine.
 * Make sure you use `rustfmt` and check compiler lints.
 * Take a look at surrounding code, and try to match your style.
 * If you implement new BPF features, please link low level
   documentation in the PR description for easier review.
 * If you implement new high-level features, make sure you have a
   minimal example either in the documentation or the `examples/`
   folder.
 * If you have a short & sweet bug fix, please 
 * Provide tests for logic changes, or things that are easy to test.
 
Following these points will help the maintainers to run through your
code and merge it in a timely manner.

Make sure the description of PR clearly explains the motivation and
link to any other resources we might need to consider when reviewing.

## What if I don't know Rust?

If you don't know Rust, and still enjoy tinkering on the project,
please take a look at our
[website](https://github.com/ingraind/ingraind.org). We welcome
contributions to the
[documentation](https://github.com/ingraind/ingraind.org/tree/master/src/content/docs),
or the
[layout](https://github.com/ingraind/ingraind.org/tree/master/src/themes/book2).

With issues regarding the website, please open a PR on the [website repository](https://github.com/ingraind/ingraind.org).
