# DITA-OT Plugin (Intro)

This project introduces **DITA Open Toolkit (DITA-OT)** customization using
a simple plugin structure.

The goal of this project is not to build a complex publishing pipeline, but to understand how DITA content is turned into output formats such as
HTML and how that output can be customized.

------------------------------------------------------------------------

## What is DITA-OT?

DITA Open Toolkit (DITA-OT) is the standard open-source publishing engine
used to transform DITA content into outputs such as:

- HTML
- PDF (via additional processors)
- Eclipse Help
- Other structured outputs

DITA-OT is a key part of real-world structured documentation workflows.

------------------------------------------------------------------------

## What is a DITA-OT plugin?

A plugin in DITA-OT is a small package that can:

- add new transformation types
- override or extend templates
- add custom resources (for example CSS, XSL, images)
- adjust how output is generated

Plugins allow teams to customize outputs without changing source topics.

------------------------------------------------------------------------

## What this project demonstrates

This project contains:

- a small DITA map (`sample.ditamap`)
- two DITA topics
- a minimal DITA-OT plugin that injects a custom CSS file into HTML output

The customization adds a footer line at the bottom of generated HTML pages.

------------------------------------------------------------------------

## How to use (high level)

1. Install DITA-OT locally
2. Copy the plugin folder into your DITA-OT `plugins/` directory
3. Run the plugin install command
4. Build HTML output using the sample map

Example (commands may vary based on your setup):

- Install plugins:
  `dita --install`

- Build HTML:
  `dita -i sample.ditamap -f html5 -o out`

After publishing, open the HTML output and confirm the footer style is applied.

------------------------------------------------------------------------

## Notes

This is a deliberately small and beginner-friendly customization that
demonstrates how publishing customization works in DITA workflows.
