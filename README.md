# Practicing Visual Enhancements

> Enhancing an exising project with visual improvements.

For this project, we will revisit the Datamuse API to enhance the search tools
we worked with a few projects ago. We will present one search with multiple
options, and we will allow users to save their results to a "Word List" so they
can more effectively browse for words.

This project is mostly built, but it requires some love and affection by way of
visual enhancements to make it more useful. With such a complex search tool, it
is possible for users to get no results. When that happens, we don't want them
to think the application has malfunctioned.

We are also updating information in the search results and in the sidebar Word
List. We want to use messages and animation to help users identify when data in
these areas of the page has changed.

To make it a little easier to create professional quality animations, we will
rely on the [`vue2-animate` project](https://github.com/asika32764/vue2-animate),
which makes a set of common animations available for use with Vue.js transition
components. We will also use a load spinner from Spinkit.

## Basic Requirements
To complete this project, we must fulfill the following requirements.

- [X] Use the `showSpinner` value to modulate the display of the `CubeSpinner` component when appropriate
- [X] Add an animation to the items of the WordList for when new items are added and removed
- [X] Add an animation to the items of the results list when a search is completed
- [X] Add messaging to results display area let the user know when no results are found
- [X] Add global messaging child component (`MessageContainer`) to `WordSearch` component
- [X] Add a global "success" message to let the user know that a word has been successfully added to the WordList
- [X] Add a global "info" message to let the user know when they try to add a word to the WordList that has already been added
- [X] Add a global "success" message to let the user know that a word has been successfully removed from the WordList
- [X] Add a global "error" message to display any errors from the API request (aside from "no results found")

## Stretch Goals
If we crave more challenges, try tackling some of these suggestions.

- [ ] Try making custom animations for everything, and don't use `vue2-animate` animations at all
- [ ] Add a shuffle feature to the wordlist along with the accompanying animation
- [ ] Make other layout or design improvements that help the application be more helpful to our users

## Build Setup for Project

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader). This project uses [`vue2-animate`](https://github.com/asika32764/vue2-animate) and [SpinKit](http://tobiasahlin.com/spinkit/).
