# CSS Formatting

CSS syntax is made up of two parts: 
the **selector** and the **declaration block** 
inside curly brackets. 

Inside the declaration block you can have multiple 
declarations. 

Each declaration is made of two parts — the property and the value:

```CSS
p {
  font-face: Georgia, Tahoma; 
  color: #ffcc00; 
}
```

In this example:

- `p` is the selector.
- `{font-face: Georgia, Tahoma; color: #ffcc00; }` is the declaration block.
- `font-face: Georgia, Tahoma; and color: #ffcc00;` are separate declarations.
- `font-face` is a property and `Georgia, Tahoma` is its value.
- `color` is a second property and `#ffcc00;` is its value.

## Put every selector in new line

Simplify merge conflicts resolution and improve readability.
Comma character is small - anyone can miss it while reading the code.

```CSS
.main-menu,
.user-menu,
.sidebar-menu {
  ...
}
```

## Use shorthand notation and order declarations alphabetically

Browser vendor prefixes are the exception for this
rule - put them wherever they work.

```CSS
.intro {
  border: 1px solid #000;
  margin: 0 10px;
  padding: 10px;
}
```

## Put single blank line after every declaration block

Just to make code more readable.

## Use 2 spaces to indent code

Just to keep the code more narrow.

# Exercises

1. Open WebStorm
2. Go to: `Preferences / Editor / Code Style / CSS`
3. Change `Tab size`, `Indent` and `Continuation indent` from 4 to 2
4. Open your project
5. Create new branch from `develop`
6. Fix CSS files according to rules above
7. Commit, push and create pull request
8. Go to github.com, accept the PR and merge it