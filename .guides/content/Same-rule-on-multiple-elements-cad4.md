Now we have seen ids and classes and it gives us a lot more power for the css.
We have also seen that we shouldn't abuse them.
Here are some examples of doing the same thing with our without classes and how to combines rules for multiple elements.

Let's imagine we have the following html :

```html
<h1 class="myfont"> My nice title </h1>
<h2 class="myfont"> My nice subtitle </h2>
<p class="myfont"> My nice paragraph </p>
```

and the css :

```css
.myfont {
  font-family: Verdana, Arial, sans-serif;
}
```

That works .. But do we really need a class for this ?

We could just do :

```html
<h1> My nice title </h1>
<h2> My nice subtitle </h2>
<p> My nice paragraph </p>
```

and

```css
h1 { font-family: Verdana, Arial, sans-serif; }
h2 { font-family: Verdana, Arial, sans-serif; }
p { font-family: Verdana, Arial, sans-serif; }
```

For the same result !
But there is a lot of repetition in there ...
This would be better :

```css
h1, h2, p { font-family: Verdana, Arial, sans-serif; }
```

Here we say that we want this font-family on h1, h2 and p.

The `,` in a css file allows us to target multiple selectors at once.

So `h1, h2, p` means : put this style on `h1`, `h2` and `p`.


