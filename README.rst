What is this
============
This is a nikola `shortcode` plugin to embed a source file to an article.

Requirements
============
- Nikola

  - I tested only nikola version 8.

Usage
=====

Setup
-----

1. Make a `plugins/` directory or the other one according to the config you specified. (e.g. `EXTRA_PLUGINS_DIRS`)
2. Put this plugin (this repository) on the plugins directory.

  .. code-block:: shell
  
    $ git clone https://github.com/righ/nikola-codeblock-shortcode.git plugins/codeblock_shortcode

  You don't have to do the operation everytime.
  It is recommended committing the plugin as yours. (it does not matter that is git submodule or not)

Description in a post
---------------------
You have to write `codeblock` short code as follows:

.. code-block:: shell

  {{% codeblock "src/server.py" label="server.py" lexer="python3" %}}


- The first argument means file path and required.
- `label` argument will appear above the code.

  - If this option is skipped, file path will be used automatically.

- `lexer` argument means a pygments short name.

  - http://pygments.org/docs/lexers/
