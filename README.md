# nut-website project

The primary goal of the Network UPS Tools (NUT) project is to provide support for Power Devices, such as Uninterruptible Power Supplies, Power Distribution
Units and Solar Controllers.

Network UPS Tools website layout is based on AsciiDoc's.
Today this is a three division CSS based layout
> It should evolve soon to a more adaptative layout.

Simulated frames using CSS (fixed banner and menu, scrolling content).
NOTE: This layout does not work with IE6.

+-----------------------------------------------------+
|          #layout-banner                             |
+--------------+--------------------------------------+
|              |                                      |
|              |                                      |
| #layout-menu |          #layout-content             |
|              |                                      |
|              |                                      |
|              |                                      |
+--------------+--------------------------------------+

Each of the three divisions is enclosed in a same-named *-box division which position and size the layout.
* The #layout-content division is a container for AsciiDoc page documents.
* Documents rendered in the #layout-content use the standard AsciiDoc xhtml11 backend stylesheets.

[specialwords]
#emphasizedwords=(?u)\\?\bNetwork UPS Tools\b
#monospacedwords=(?u)\\?\basciidoc\(1\) (?u)\\?\ba2x\(1\)



## How to play with nut-website


### How to generate nut-website

Type the following commands:

```
./autogen.sh
./configure
make
```

Then check the output folder generated, and send its content to a local web server to see results.

To clean folder after a build use:

```
make clean
```


### How to implement changes

1. A first idea is to modify directly the code sent on Webserver. You can modify
files and check changes locally as you would do for a statical website.

2. The deeper step is to check the source code
Main entry point would be web-layout.conf, the website canvas: it defines all
website commons parts, that will be integrated in all pages.
