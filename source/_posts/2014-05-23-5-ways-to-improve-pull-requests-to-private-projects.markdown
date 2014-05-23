---
layout: post
title: "5 Ways to Improve Pull Requests to Private Projects"
date: 2014-05-23 16:00
comments: false
categories: [pull requests, github, github enterprise, git]
---

At [VBrick](http://www.vbrick.com) we've hosted our private projects on GitHub
Enterprise for the last few months. Pull requests are the team's code review
step so only blessed changes end up merged into our mainline branch. Even though
team members have mixed levels of git and GitHub experience, the current
process is as lightweight as it gets -- any developer on the project can submit
or merge a pull request.

The following are some best practices I've learned from my experience using GitHub for
private as well as open source projects. Many open source lessons carry over -- 
if you think about it, submitting a pull request to Twitter Bootstrap to add
semicolons to their JavaScript<small>[[1](https://github.com/twbs/bootstrap/issues/3057)]</small>
and submitting sweeping coding style changes to your
team's project are both wastes of time.

I assume the reader has basic working knowledge of git, GitHub, and what makes
for a good commit / commit message.

## Actually use pull requests

Pull requests encourage critical discussion around code changes, improve code quality,
and increase team knowledge of the codebase. When pull requests are merged, team
members and project watchers are notified that the repository was updated with
blessed changes. What's not to like?

## Make your pull requests small and easy to review

As the contributer of a pull request, you're the expert on your changes. Therefore
to spread knowledge and receive meaningful feedback you should strive to make life
as easy as possible for reviewers.

Use a concise title. If you don't use GitHub issues, link to the issue in your
project's issue tracker. Summarize what has changed and why the changes are necessary,
particularly if the pull request is large or if the issue's implementation is not
obvious.

When possible, don't submit a massive pull request. Submit separate pull requests for
each logical set of changes. Within the pull request, strive for commits that are atomic --
that is, the commit represents a single refactoring or distinct change to the system.

## Collaborate before the pull request

Whether in person or remote, discuss the design of a feature implementation or bug fix
prior to submitting a pull request. If you're like me and find pair programming
effective, work as a pair before submitting the pull request.

## Keep the process lightweight

The freedom that any developer on my project can merge any of the project's pull
requests at times resembles anarchy. That said, assigning reviewers to
pull requests would create a bottleneck for my team. On a private project, the
contributor of a pull request is the expert on the changes and the person with
the most skin in the game to ensure the pull request is reviewed and merged
in a timely fashion.

As a developer, if you don't know who should review a pull request, ask.

## Use forks

Resist the temptation to work on separate branches in a shared repository. As
a developer, it's easier to experiment when forks are treated as sandboxes and
branches in forks considered public history is the exception rather than the rule.

<small>1. [bootstrap-dropdown.js clearMenus() needs ; at the end](https://github.com/twbs/bootstrap/issues/3057)</small>
