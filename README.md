Composer CheatSheet for developpers
====================================

[Composer](https://getcomposer.org/ "Composer") is an awesome dependency manager for PHP. 
This is a one-page-only documentation for this tool. 

There is a very nice and [well-supplied documentation](https://getcomposer.org/doc/) on the official website, this page just brings you the essential. 
If you want to learn more about this awesome tool, just go on the [official documentation](http://getcomposer.org/doc/ "official documentation").


Contributing
------------
If you find any typo, error, or you think there's a missing information, just send us a pull request!

Maintenance
-----------
- The common JoliCode footer is vendored from [jolicode/oss-theme](https://github.com/jolicode/oss-theme)
  and pasted **inline** in `index.html` (inside the `<div id="snippet-joli-footer">` block), so it renders
  without any fetch — including when opening the page from the filesystem.
  To update it, re-run this command from the repository root, re-apply the two substitutions, then replace
  the `<div id="snippet-joli-footer">` block in `index.html` with the result:
  ```
  curl -o joli-footer.html https://raw.githubusercontent.com/jolicode/oss-theme/refs/heads/main/snippet-joli-footer.html
  sed -i 's/#GITHUB_REPO/jolicode\/composer-cheatsheet/g' joli-footer.html
  sed -i 's/<!-- #SUBTITLE -->/Found a typo? Something is wrong in this documentation? Just <a href="https:\/\/www.github.com\/jolicode\/composer-cheatsheet\/blob\/gh-pages\/index.html" class="jf-link">fork and edit it<\/a>! UI powered by <a href="https:\/\/www.npmjs.com\/package\/json-schema-explorer" class="jf-link">json-schema-explorer<\/a>./' joli-footer.html
  rm joli-footer.html
  ```
- Documentation for CLI commands lives in `cli-hints.js`; schema/property docs in `composer-schema.json`.
- UI is powered by the self-hosted [json-schema-explorer](https://www.npmjs.com/package/json-schema-explorer)
  (`schema-explorer.js` / `schema-explorer.css`, MIT licensed, see `schema-explorer.LICENSE`).