# nut-website
Network UPS Tools website and protocol library

## Network UPS Tools website layout (based on AsciiDoc's).

Three division CSS based layout

Simulated frames using CSS (fixed banner and menu, scrolling content).

NOTE: This layout does not work with IE6.

Each of the three divisions is enclosed in a same-named *-box division which position and size the layout.

The #layout-content division is a container for AsciiDoc page documents.

Documents rendered in the #layout-content use the standard AsciiDoc xhtml11 backend stylesheets.

### specialwords
1. emphasizedwords=(?u)\\?\bNetwork UPS Tools\b
2. monospacedwords=(?u)\\?\basciidoc\(1\) (?u)\\?\ba2x\(1\)
