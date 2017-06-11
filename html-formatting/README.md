# HTML Formatting

## Beware indentation

Do not indent `html`, `head`, `body` and first level
of `body` children. It helps reducing indentation level
of most obvious HTML document parts, making it easier
to fit complex nesting on narrow screen.

It's common to display files side-by-side
on panoramic screens.

```HTML
<!doctype html>
<html lang="en">
<head>
  ...
</head>

<body>
<div id="menu">
  ...
</div>

<div id="header">
  ...
</div>

<div id="content">
  ...
</div>

<div id="footer">
  ...
</div>
</body>
</html>
```

## Indent code using 2 spaces - not 4

This one is subjective but considered most common. 
There is no standard way of indenting code - it's always the team
deciding which one to apply.


```HTML
<div>
  <ul>
    <li>
      <a href="#home">
        Home
      </a>
    </li>
  </ul>
</div>
```

## Put blank lines between child nodes

Do not put blank lines anywhere else.
It simply increases code readability.
Never use more than single blank line.

```HTML
<div>
  <ul>
    <li>
      One
    </li>
    
    <li>
      Two
    </li>
    
    <li>
      Three
    </li>
  </ul>
</div>
```

## Put every attribute in new line

This one makes it easier to resolve merge conflicts.
Imagine having the code in one line 
while one programmer changes `href` 
and another one changes `class` attribute
in the same time.

```HTML
<a href="#team" 
   title="Team"
   class="menu--item__active"
   >...</a>
```

## Use comments wisely

You should use comments whenever you do not obey those rules on
purpose. Always put there a proper explanation.

Do not leave "dead code" in comments if you don't describe why
it's there in the first place.

Don't be afraid of deleting code - you use Git and you can
browse the history anytime you want to bring some code back
from darkness ;)

Using comments like `<!-- begin / end of features section -->` is
mostly useless since you have `id` and powerful IDE capable of
highlighting closing tags.

The best code is no code at all.

## Simplify id naming

Use lowercase names and dashes.

```HTML
<div id="team-members">
  ...
</div>
```

> Warning! 
> Changing id value may break your website if 
> you use it in CSS. You should change your CSS
> accordingly.

# Exercises

1. Open WebStorm
2. Go to: `Preferences / Editor / Code Style / HTML`
3. Change `Tab size`, `Indent` and `Continuation indent` from 4 to 2
4. Open your project
5. Create new branch from `develop`
6. Fix HTML files according to rules above
7. Commit, push and create pull request
8. Go to github.com, accept the PR and merge it

If all PR are correct you can merge all of them but merging one
will do the job too.

Remember that you can use `Code / Reformat Code` option




