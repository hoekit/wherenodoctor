WHERE THERE IS NO DOCTOR
---
A Village Health Care Book

_Open Sourced in 1977 by [David Werner](http://davidbwerner.info/), Carol Thuman, Jane Maxwell
(orignal title: Donde No Hay Doctor ISBN	978-0-942364-15-6)_


![app logo](screen.png)


# Status:
- Many chapters to be completed
- Chapters with full text: **[1,2,3,4,5]**
- Chapters with all links working: **[content]**


# 2do
- **search for a better [search](https://github.com/olivernn/lunr.js)** maybe [lunr.js](http://lunrjs.com/) - Using at the moment [jekyll-search](https://github.com/christian-fei/Simple-Jekyll-Search), but it just get chapter titles! NOT ENOUGH! no way to make 'content' work...
- [ ] Make it easily translatable.

# Done:
- [X] setup [upup.js](https://github.com/TalAter/UpUp)
- [X] squeezed all chapters into one single page.
- [X] mobile friendly version one pager.
- [X] inital collection of PDF release.
- [X] logo. _thanks to david@[work-it](http://work-it.it)_
- [X] github repo.
- [X] https. _[check](https://junglesta.github.io/wherenodoctor/)_
- [X] auto-TOC for each chapter

# Source:

## Where There Is No Doctor
The most widely-used health care manual for health workers, educators, and others involved in primary health care and health promotion around the world. Current edition includes updated information on malaria, HIV, and more.


In the Journal of the American Medical Association, a 2010 review said,

>it is still not known if the book effectively improves health. [However,] In most of the world, where physicians are not available and diseases are rampant, the status quo is unacceptable. Until better solutions are created, Where There is No Doctor is probably a useful stop-gap measure. [read more on jamanetwork](https://dx.doi.org/10.1001%2Fjama.2010.244)

[read more on wikipedia](https://en.wikipedia.org/wiki/Where_There_Is_No_Doctor)

Firstly published in 1977 by [hesperian.org](http://hesperian.org/books-and-resources/)

![cover] (https://upload.wikimedia.org/wikipedia/en/f/f9/Where_There_Is_No_Doctor_book_cover%2C_13th_revised_printing.jpg)


## dev
```sh
jekyll serve --watch --trace --baseurl ''
```

#### Minimal necessary formatting logic / make sure

**Page no. anchors**

`#[page-..` needs to read `#[page-` (with space after `#`)

**Table of Content**

auto-TOC: put this at top

```sh
* TOC
{:toc}
```
and this to stop including in ToC

```sh
{:.no_toc}
```

**logic for headers**

`h1` will be UPPERCASED by css.

`h2` need be lowercase and have a `.` at the end when phrases.

`h2` can be uppercase when short names and not phrases.
