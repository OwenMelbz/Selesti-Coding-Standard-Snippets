# Selesti coding standard snippets

A collection of snippets we use to help enforce certain coding standards. Based off our blog post https://www.selesti.com/blog/how-selesti-handle-their-code-standards

It will not be suitable for everybody, but its tuned for our laravel 5 projects on macOS which we use sass.

It assumes you have eslint, sass-lint, phpcs installed and accessibly globally. Additionally we have a bitbucket pipeline check.

## Prerequisite
- Make sure you have `eslint` installed globally, confirm with `which eslint` or install with `npm install eslint -g`
- Make sure you have `sass-lint` installed globally, confirm with `which sass-lint` or install with `npm install sass-lint -g`
- Make sure you have `php` installed globally, confirm with `which php`
- Make sure phpcs is included with your project e.g `composer require squizlabs/php_codesniffer` or globally (update the git hooks)

## Usage
- Add the contents of the `scripts` array into your `composer.json` - this contains some helpers like `composer run clean`, `composer run psrcheck` etc
- Copy the "git-hooks" folder to your project root, then install them by typing `composer run githooks` this will symlink them so they run automatically when you pull or push
- Place the rest of the rule files in the root of your project

## Customisation
- You can edit the rule files to suit yourself
- You can update the paths inside the git-hooks folder

# Enjoy :)
Any questions just add an issue and we'll get back to you when possible!
