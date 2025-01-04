
OpenOMF Translations
====================

These text documents contain translations for [OpenOMF],
a remake of One Must Fall 2097.

[OpenOMF]: https://github.com/omf2097/openomf
[openomf sourcecode repo]: https://github.com/omf2097/openomf


Current Status
--------------

[ENGLISH.TXT](ENGLISH.TXT): Complete.  
[GERMAN.TXT](GERMAN.TXT): Mostly complete, but has no maintainer and a few strings in English.  
[DANISH.TXT](DANISH.TXT): Low quality, low effort, machine translation.  


Translators Guide
-----------------

TODO: Write a guide on how to contribute a translation.

TLDR; copy ENGLISH.TXT, make your changes, and open a pull request.


Programmers Guide
-----------------
Note that this repo is included in openomf as a submodule.

To add a language string to this repo:
- Add the new language string to each language TXT in this repo.
Using English as a placeholder is fine, so long as you leave a comment
`# TODO: Translate ...`
- Update the [`langstr_count` file] with the new number, so the CI pipeline can pass.  
Please note: language strings are 0-indexed, so if your last lang str ID is 457, the count is 458.
- Open a pull request to this repo with the above changes.

[`langstr_count` file]: langstr_count

To add a language string to the [openomf sourcecode repo]:
- Add the translation to [`LanguageStrings.cmake`]
- Update the [`translations` submodule], with required modifications described above.

[`LanguageStrings.cmake`]: https://github.com/omf2097/openomf/blob/master/cmake-scripts/LanguageStrings.cmake
[`translations` submodule]: https://github.com/omf2097/openomf/blob/master/resources
