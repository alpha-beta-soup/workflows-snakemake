# Workflow Engines

This lesson is focused on teaching the basics of two modern workflow engines: [Snakemake](https://snakemake.readthedocs.io/en/stable/) and [Nextflow](https://www.nextflow.io/).

After completing this lesson you should have a good understanding of the role
of workflow engines and the value they can bring to complex data processing.
Additionally, by implementing the same workflow in two different systems, you
will start to understand some of the strengths and limitations of each.
Hopefully this will help you choose the best approach for your work.

There are 2 primary components to this lesson. Each component is budgeted
half a day's worth of teaching-time, resulting in a one day workshop.

1. Snakemake
2. Nextflow

In each section we will implement the same data processing pipeline. This gives the best opportunity to compare the two approaches.

The example workflow performs a frequency analysis of several public domain books sourced from [Project Gutenberg](https://www.gutenberg.org/), testing how closely each book conforms to [Zipf's Law](https://en.wikipedia.org/wiki/Zipf%27s_law). All code and data are provided. This example has been chosen over a more complex scientific workflow as the goal is to appeal to a wide audience and to focus on building the workflow without distraction by the underlying science.

## Topic breakdown and todo list

The lesson outline and rough breakdown of topics is in
[lesson-outline.md](lesson-outline.md).

## Lesson writing instructions

This is a fast overview of the Software Carpentry lesson template.

For a full guide to the lesson template, see the
[Software Carpentry example lesson](http://swcarpentry.github.io/lesson-example/).

### Lesson structure

Software Carpentry lessons are generally episodic, with one clear concept for each episode
([example](http://swcarpentry.github.io/r-novice-gapminder/)).
We've got 2 major sections, each section should be broken up into several episodes.

An episode is just a markdown file that lives under the `_episodes` folder.
Here is a link to a [markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) with most markdown syntax.
Additionally, the Software Carpentry lesson template uses several extra bits of formatting - see here for a [full guide](http://swcarpentry.github.io/lesson-example/04-formatting/).
The most significant change is the addition of a YAML header that adds metadata (key questions, lesson teaching times, etc.)
and special syntax for code blocks, exercises, and the like.

Episode names should be prefixed with a number of their section plus the number of their episode within that section.
This is important because the Software Carpentry lesson template will auto-post our lessons in the order that they would sort in.
As long as your lesson sorts into the correct order,
it will appear in the correct order on the website.

### Publishing changes to Github + the Github pages website

The lesson website is viewable at [https://csiro-data-school.github.io/workflows/](https://csiro-data-school.github.io/workflows/).

The lesson website itself is auto-generated from the `gh-pages` branch of this repository.
Github pages will rebuild the website as soon as you push to the Github `gh-pages` branch.
Because of this `gh-pages` is considered the "master" branch.

### Previewing changes locally

Obviously having to push to Github every time you want to view your changes to the website isn't very convenient.
To preview the lesson locally, run `make serve`.
You can then view the website at `localhost:4000` in your browser.
Pages will be automatically regenerated every time you write to them.

Note that the autogenerated website lives under the `_site` directory
(and doesn't get pushed to Github).

This process requires Ruby, Make, and Jekyll. You can find setup instructions [here](http://swcarpentry.github.io/lesson-example/setup/).

## Example lessons

A couple links to example SWC workshop lessons for reference:

* [Example Bash lesson](https://github.com/swcarpentry/shell-novice)
* [Example Python lesson](https://github.com/swcarpentry/python-novice-inflammation)
* [Example R lesson](https://github.com/swcarpentry/r-novice-gapminder) (uses R markdown files instead of markdown)