# General

The Ember blog is the official news outlet of the Ember Learning Core team. You can publish new posts by adding a markdown file (`.md`) to the `content` directory.

## Ember Times

The Ember Times is a blog newsletter with weekly updates from the Ember land.
It is part of the [Emberjs.com](https://emberjs.com/) website and managed by the Learning Team and friends.

### Contributing

Anyone can become an Ember Times editor. The best way to start is to join [#support-ember-times](https://discordapp.com/channels/480462759797063690/485450546887786506) channel on [Ember Community Discord](https://discordapp.com/invite/zT3asNS). New blog posts are released every Friday.

The process to publish a new weekly post is as follows:

- The championing editor of the week creates a branch with the MD file containing next week's Ember Times post
- Editors will then pull request against that branch with changes to that file
- Once the new blog post file is complete, the newly created branch is merged back into the website
- As a last step, the content is copied over to [Goodbits](https://the-emberjs-times.ongoodbits.com/), which is the tool currently being used to send the newsletter and manage its subscriptions

The Reader's Questions section of the newsletter is usually answered by core team members, but anyone can give a helping hand.
The answers are posted on [discuss.emberjs.com](https://discuss.emberjs.com/) and linked back to the weekly blog post.

### Writing Style Guide

- Use `Sentence case` for section headings, but feel free to capitalize proper nouns! 
- Please add an emoji at the end of your title, if you're having trouble finding an emoji use a search tool like [https://emojipedia.org/](https://emojipedia.org/).
- In general, refer to people by their GitHub handle, e.g. `[Your Name (@your_name_here)](https://www.github.com/your_name_here)`. (If the person is mentioned more than one time in the same paragraph, feel free to deviate after one @ mention!.)
- We tend to refer to `Ember`, `Ember Data`, and `Ember CLI` as their name (versus the repo name) because we mention them so often. For most other repos, use the repo name e.g. `[machty/ember-concurrency](https://github.com/machty/ember-concurrency)`.
- The word `addon` is usually denoted as lowercase and as a single word.
- Add your name to the author list at the bottom of the Times when submitting a PR for the week.

### Goodbits

To prepare the newsletter broadcast on Goodbits the following steps are necessary:

- Log into Goodbits
- From the list of emails, duplicate one of the latest entries to create a new draft one
- Edit the blocks from the newly duplicated draft, with the new blog post content
- Select 'Prepare to send'
- Choose the option 'Send later' and schedule it to Friday 9 PM UTC

### What Is New in Ember Land

There is a tool available to gather the weekly contributions on Ember repos and to generate the contributors' list, here: [what-is-new-in-emberland](https://github.com/jessica-jordan/whats-new-in-emberland). It's an Ember app 🐹, you can simply download, build it and serve it!

### Pushing Your Changes to the Blog Post

A typical Git forking workflow can be used to contribute:

- Fork this repo
- Clone the repo in your own machine
- Set upstream: `git remote add upstream https://github.com/ember-learn/ember-blog`
- Fetch upstream: `git fetch upstream`
- Switch to the most current Ember Times branch, they usually follow the format: `blog/embertimes-#`

For example, switch to this branch for issue 92: `blog/embertimes-92`

```bash
git switch -t upstream/blog/embertimes-165 # or, git checkout blog/embertimes-165
```

- Find the latest blog issue template at `content/the-ember-times-issue-#.md`

For example: `2019-04-05-the-ember-times-issue-92`

Add your section to the template. You'll see useful notes in the blank sections:

```md
## [Section Title in Title Case 🐹](#section-url)
<change section title emoji>
<add your name to author list, top and bottom>
<add blurb and emoji to "SOME-INTRO-HERE">
```

- Use `git` to add your file and commit changes:

```bash
git add .

git commit -m "you-commit-message-here"
```

- Push changes, you may have to set your upstream origin first:

`git push --set-upstream origin blog/embertimes-#`

- Create a pull request from your repo on Github.

There should be an open pull request titled: `[WIP] The Ember Times No. #` Please include reference to this PR in your pull request.

For example: "Add a section to Ember Times [`#46`](https://github.com/ember-learn/ember-blog/pull/46)"

Thank you for contributing to Ember Times!

## DecEmber

In December 2019 we are organising a blog series featuring an interesting addon each day. If you want to contribute, please claim one of the `December` issues in the [`ember-learn/ember-blog` repository](https://github.com/ember-learn/ember-blog/issues?q=is%3Aissue+is%3Aopen+december) and review [our December Contribution Guide to get started!](https://github.com/ember-learn/ember-blog/blob/master/post-templates/december-2019-template.md)
