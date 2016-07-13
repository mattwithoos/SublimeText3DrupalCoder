Sublime Text 3 integration with Drupal Code Sniffer.

1. Install Drupal Coder (https://packagist.org/packages/drupal/coder#user-content-installation)
2. Make a note of the install location of phpcs (i.e. /Users/yourusername/.composer/vendor/bin)
 2. If phpcs was previously installed, uninstall and redo Drupal Coder installation (phpcs comes with it)
3. Clone this repo somewhere:
`git clone https://github.com/mattwithoos/SublimeText3DrupalCoder
4. *IMPORTANT* Edit DrupalCoder.sublime-build, updating the path /Users/changeme/... to phpcs. You can try `whereis phpcs` or `which phpcs` if you don't have the path from step 2.
5. Place the DrupalCoder.sublime-build file into your Packages/User directory.
   (On OS X this is ~/Library/Application Support/Sublime Text 3/Packages/User)
6. Open up Sublime Text 3 and select Tools > Build System > DrupalCodingStandard
7. Open any Drupal file and hit Cmd+B (probably CTRL+B on Windows/Linux)
8. You can make reporting more compress with "--report=full". In this case sniffer will show only line number(without full path to file)
9. To auto fix any file with phpcbf run Cmd+shift+B (probably CTRL+shift+B on Windows/Linux)

Got Sublime Text 2? Credits to sirkitree for the inspiration, some of the readme and code, as well as having a Sublime Text 2 build script. https://github.com/sirkitree/DrupalCodingStandard
