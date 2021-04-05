Guide to new contributors
=========================

Thanks for contributing to `ingraind` and RedBPF!

Before delving into the best way to participate in the project, please
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
asked to make some changes to the code.

In case you are not certain that your code quality or the feature
you're implementing is suitable for the project, please open an issue
with the question, or send the PR anyway.
This allows the maintainers to give you hands on feedback, and
highlight anything you may not have considered.

A quick list of things maintainers will check during review.
The following 3 steps are requirements for all PRs:

 * All public API items should have documentation.
 * Don't break public APIs unnecessarily.
 * Make sure you use `rustfmt` and check compiler lints.
 
Additionally, please pay attention to the following points as it helps
with our review. However, these are _not_ required:

 * Adding new API items is generally fine.
 * Take a look at surrounding code, and try to match your style.
 * If you implement new BPF features, please link low level
   documentation in the PR description for easier review.
 * If you implement new high-level features, make sure you have a
   minimal example either in the documentation or the `examples/`
   folder.
 * If you have a short & sweet bug fix, please create a PR and
   mention ways to reproduce or scenarios when the bug appears.
 * Provide tests for logic changes, or things that are easy to test.
 
Following these points will help the maintainers to run through your
code and merge it in a timely manner.

Make sure the description of the PR clearly explains the motivation
and link to any other resources we might need to consider when
reviewing.

# Developer Certificate of Origin

The [`DCO GitHub plugin`](https://github.com/apps/dco) is enabled on
all repositories in the `ingraind` organization. This plugin will
check if *all* your commits in a PR have signed off on the Developer
Certificate of Origin.

A sign-off looks like this at the end of your Git commit message:

	Signed-off-by: Peter Parkanyi <peter@redsift.io>


Having this line appended to your commits proves that you agree to the
following document:


	Developer Certificate of Origin
	Version 1.1

	Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
	660 York Street, Suite 102,
	San Francisco, CA 94110 USA

	Everyone is permitted to copy and distribute verbatim copies of this
	license document, but changing it is not allowed.


	Developer's Certificate of Origin 1.1

	By making a contribution to this project, I certify that:

	(a) The contribution was created in whole or in part by me and I
		have the right to submit it under the open source license
		indicated in the file; or

	(b) The contribution is based upon previous work that, to the best
		of my knowledge, is covered under an appropriate open source
		license and I have the right under that license to submit that
		work with modifications, whether created in whole or in part
		by me, under the same open source license (unless I am
		permitted to submit under a different license), as indicated
		in the file; or

	(c) The contribution was provided directly to me by some other
		person who certified (a), (b) or (c) and I have not modified
		it.

	(d) I understand and agree that this project and the contribution
		are public and that a record of the contribution (including all
		personal information I submit with it, including my sign-off) is
		maintained indefinitely and may be redistributed consistent with
		this project or the open source license(s) involved.

To make the developer process more efficient, you can use the `git
commit -s` command instead of your usual `git commit` command line to
automatically append the sign-off line to every commit you make.

You can also make this the default behaviour by changing your Git config:

	git config --add alias.amend "commit -s --amend"
	git config --add alias.c "commit -s"

### Fixing DCO errors

If a single commit doesn't contain the sign-off line, the CI will not
allow your PR to be merged.

You will need to `git push --force` to the PR with the amended commit
messages to fix this error.

Alternatively, you can squash the commits to add the sign-off line, assuming you
diverged your branch from `main`, like so:

	git rebase -i main # interactive squash
	git push origin -f

## What if I don't know Rust?

If you don't know Rust, and still enjoy tinkering on the project,
please take a look at the [repository](https://github.com/ingraind/ingraind.org) for our
[website](https://ingraind.org). We welcome
contributions to the
[documentation](https://github.com/ingraind/ingraind.org/tree/master/src/content/docs),
or the
[layout](https://github.com/ingraind/ingraind.org/tree/master/src/themes/book2).

With issues regarding the website, please open a PR on the [website repository](https://github.com/ingraind/ingraind.org).
