=== CodeHighlighter ===
Contributors: blobaugh,iwongu,NikV
Tags: post, formatting, syntax highlight, code highlighter
Requires at least: 2.0
Tested up to: 3.7.1
Stable tag: 1.9

This plugin is a syntax highlighter for source code using GeSHi.

== Description ==

This plugin is a syntax highlighter for source code. It uses *GeSHi* as fontifier engine.

= Usage =

1. Put the code snippet in a `<code>` tag.
1. Add the lang attribute to the code tag like the following. `<code lang="php">` 
1. Add the lineno attribute to the `<code>` tag after the lang tag if you wish to start at a line other than 1. `<code lang="cpp" lineno="42">`
1. If you do not add lang attribute, the `<code>` tag is handled normally.
1. If you want to have border, add the style like the following to your .css file. `code { border: 1px dotted #ccc; padding: 0.2em 0.5em; }`
1. You can use following languages in lang. `abap, actionscript, ada, apache, applescript, asm, asp, autoit, bash, blitzbasic, bnf, c, c_mac, caddcl, cadlisp, cfdg, cfm, cpp-qt, cpp, csharp, css-gen, css, d, delphi, diff, div, dos, dot, eiffel, fortran, freebasic, genero, gml, groovy, haskell, html4strict, idl, ini, inno, io, java, java5, javascript, latex, lisp, lua, m68k, matlab, mirc, mpasm, mysql, nsis, objc, ocaml-brief, ocaml, oobas, oracle8, pascal, per, perl, php-brief, php, plsql, python, qbasic, rails, reg, robots, ruby, sas, scheme, sdlbasic, smalltalk, smarty, sql, tcl, text, thinbasic, tsql, vb, vbnet, vhdl, visualfoxpro, winbatch, xml, xpp, z80` 

**Note:** Version 1.9 adds support for `<code>` tags, however to ensure backwards compatibility support for the `<pre>` tag will not be removed.


== Installation ==

1. Unzip the plugin archive.
1. Upload the directory to the `/wp-content/plugins/` directory
1. Activate the plugin through the 'Plugins' menu in WordPress

== Known issues ==

1.  Because this plugin uses regular expression to match string range from `<code lang="some">` to `</code>`, you can't use `</code>` in your code snippet. If you must put the `</code>` tag, you can put a space between `<` and `/code>` like `< /code>`. The `< /code>` is converted to `</code>` automatically by plugin.
1. If you want to change the style, you should modify the plugin source file. :-P

== Changelog ==
== 2.0 ==
*Updated functionality to 3.7.1

= 1.9 =
* Added plugin maintainer
* Removed outdated links
* Added support for the `<code>` tag
* Fixed several HTML entity display issues
* Line numbering now defaults to displaying line numbers starting at 1

