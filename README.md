# GitHub Battle (Hooks)

I created this project while completing [Tyler McGinnis' "React Hooks" course](https://tylermcginnis.com/courses/react-hooks/).

## About

"GitHub Battle" is a React application that pulls repository and user data from the GitHub API and displays popular repositories categorized by language (JavaScript, Ruby, Java, CSS, Python). The Battle component allows users to input two GitHub usernames and "battle" to see who has a better score/profile. These functions take in the data and calculate each GitHub user's score:

`function getStarCount(repos) { return repos.reduce( (count, { stargazers_count }) => count + stargazers_count, 0 ); }`

`function calculateScore(followers, repos) { return followers \* 3 + getStarCount(repos); }`

This project refactors the ["GitHub Battle" app](https://github.com/jenross/github-battle-react) I created while completing Tyler McGinnis' "React" fundamentals course, which employed class component architecture. After learning how to implement custom hooks and built-in Hook API's (including useState, useEffect, useContext, useReducer, useCallback, useMemo, and useRef), I removed all of the class components and replaced them with functions/hooks.

## Demo

Fetch popular repos

![](popular_githubbattle.gif)

Battle

![](battle_githubbattle.gif)

## Peruse/Play

Check out the app [here](https://githubbattlehooks.netlify.com/).
