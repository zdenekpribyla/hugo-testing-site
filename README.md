# TASK to DO

Hugo version v0.55.6/

Please do not move existing `range` function and `partial` from one .html to another .html. This file structure is imitation of my real project. It has to be stay the same.

On `product-review` page, there is function which calls products defined in `front matter` in `product`. And render some of their values (via partial `single-review`).

## Task

1) Counter
On list.html page (probably there..), create function which add number of order for every listed product. So the Car with number 1, Chair with number 2, Shavel with number 3

2) Show ingredients
there is data file `ingredients.yaml` and each product is composed of some of them. In partial `single-review` I need to render every ingredient, which is placed in product (see data file products.yaml)

3) One data file
And finally, I want to keep all data in one file called `alldata.yaml`
1,2,3 Done

4) Table of Content for all headings
I have put another partial `call-products` (just for removing `range` from `list.html`). And add some new heading element in `list.html`
Now I need to display a `Table of Contents` for every `H` headings element on `/product-review/` page. Now it is working just for `.Content` headings.
Done

5) Separate Table of Content (ToC)
I moved ToC to separate partial `toc.html` to get greater freedom with placing ToC in layout. Please check if it is OK like that.

6) extend Table of Content for H3
I add some h3 headings to _index.md and I need them to display in ToC (and of course behind the correct H2).
Leave this task for now

7) include other H2 in layout to ToC
See list.html. I add new H2 element `This heading is not in ToC` directly hardcoded in layout. But this heading is not included in ToC. Just take a look if there is some easy solution. If not, just go away. This is not critical function.

8) Single product review in text
Sometimes, I need to put single product review directly in the middle of .md text (between headings).
See _index.md to understand what I mean ( I commented out ). So call product via shortcode `render-single-review.html` and after it has to be ranged and renderd by `single-review.html` (yes, we can use special partial for that, but it would be duplicity of single-review.html more less).
I have error with `<add .index 1>` so try to find solution.
