## Become a contributor

### Git flow

We use a custom Git flow which is based on the feature branches. Before you jump into styling, name your branch according to these rules:

- When developing a new Global Styles: `git checkout -b feature/someGlobalStylesName`.

Always create your branch off master. When you're ready, just create a pull request. Remember to rebase onto `master` before requesting a code review in your pull request (`git rebase origin/master -i` and follow the instructions). You'll find more details in a pull request description template.
