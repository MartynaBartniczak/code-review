# Naming CSS Classes

## BEM

Basic BEM (Block-Element-Modifier) idea is to separate
user interface into components, define possible variants
of its styling and name all of it.

The resulting code is more verbose but it is not an issue since
we can generate most of it using `SASS` and compress the resulting
files using `gzip` on server side (it handles duplicate names 
optimization perfectly).

```HTML
<div class="editor">
  <ul class="editor--palette palette">
    <li class="palette--option">...</li>
    <li class="palette--option__active">...</li>
    <li class="palette--option__disabled">...</li>
  </ul>
  
  <div class="editor--viewport">
    ...
  </div>
</div>
```

```CSS
.editor {

}

.editor--palette {

}

.editor--viewport {

}

.palette {

}

.palette--option {

}

.palette--option__active {

}

.palette--option__disabled {

}

```

- [https://en.bem.info/](https://en.bem.info/)
- [http://getbem.com/](http://getbem.com/)
- [Mindbemding](http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/)