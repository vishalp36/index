# Contributing

This is mostly automated.

## Make your own

1. Create an `index` repo
2. Visit the Repositories tab on your profile
3. Run this in the console, it will copy some markdown to jump start the repo:

  ```js
  copy($$('.source').map(repo => {
    const name = repo.querySelector('.repo-list-name');
    const desc = repo.querySelector('.repo-list-description');
    return `* [${name.innerText}](${name.firstElementChild.href}) - ${desc && desc.innerText}`
  }).join('\n'))
  ```

4. Create README.md file with the contents of your clipboard
5. Setup this [IFTTT recipe](https://ifttt.com/recipes/455946-remind-me-to-add-my-new-repo-to-my-github-index) to automatically remind you to add new repos by creating new issues.