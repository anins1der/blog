---
title: "template post that i will use"
excerpt_seperator: "<><><>"
categories:
  - blog
  - template
tags:
  - blog formatting
  - template
---
# title has to be in **YYYY-MM-DD-name.file-extension** format or it wouldn't work

# notices is a great way to tell smth about a thing!

how i need to do this? (the answer is **yes**)
lol jk

so i need to add this(`{: .notice}`) to end of the pharagraph, huh?
k lemme try all of these:

actually, this is a pharagraph. but adding `{: .notice}` end of it caused this cool look :)
{: .notice}

**Changes in Service:** We just updated our [privacy policy](#) here to better service our customers. We recommend reviewing the changes.
{: .notice}

this is the "*primary*" version of above? what?? it's just darker :'(
{: .notice--primary}

**info**: 2+2 is 5, actually :))
{: .notice--info}

**warning!**: you are SO KOOOOLLL!!!
{: .notice--warning}

ooohh i just launched a **nuke** to the moon and this happened :/
{: .notice--danger}

and i *succesfully* **nuked** the cheesy moon :D
{: .notice--success}

you should use html with `markdownify` and you're good to go!

```html
{% raw %}{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages (in your dreams)
* Drafts will now auto-save while writing (wat i need dis)
{% endcapture %}{% endraw %}

<div class="notice">{% raw %}{{ notice-2 | markdownify }}{% endraw %}</div>
```

which does this:

{% capture notice-2 %}
#### New Site Features

* You can now have cover images on blog pages
* Drafts will now auto-save while writing
{% endcapture %}

<div class="notice">
  {{ notice-2 | markdownify }}
</div>

or i can just do it in "just HTML" style :D

```html
<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>
```

which does this:

<div class="notice">
  <h4>Message</h4>
  <p>A basic message.</p>
</div>

# quotes/notes/captions/whatever tf is this is a **great way** to show smth, too!

and i just need to insert a `>` at the beginning of the sentence

> woooohooooooooo

> a quote in a notice :D {: .notice--success}

and do not **EVER** try to rickroll someone (or else >:[)
only i can rickroll[:](https://www.google.com/url?sa=t&source=web&rct=j&opi=89978449&url=https://www.youtube.com/watch%3Fv%3DdQw4w9WgXcQ&ved=2ahUKEwifouzLptaGAxUUDHkGHTISBzQQ78AJegQIHBAB&usg=AOvVaw0aHtehaphMhOCAkCydRLZU)

# you can use both markdown and html in harmony thanks to `kramdown`!

[go up](#)