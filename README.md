`#sass` `#css` `#html` `#master-in-software-engineering`

# SASS - Clone Instagram <!-- omit in toc -->

<p>
  <img alt="Version" src="https://img.shields.io/badge/version-1.0-blue.svg?cacheSeconds=2592000" />
</p>

> Sass (which stands for 'Syntactically awesome style sheets) is an extension of CSS that enables you to use things like variables, nested rules, inline imports and more
>
> The purpose of this project is to learn the basics of SASS and put them into practice by building a visual replica of Instagram

## Index <!-- omit in toc -->

- [Requirements](#requirements)
- [Repository](#repository)
- [Technologies used](#technologies-used)
- [Project delivery](#project-delivery)
- [Resources](#resources)

## Requirements

- You must use variables at least once in the project.
- You must use nesting.
- You must use inheritance at least once in the project.
- You cannot use third party libraries for the development of this pill

## Repository

First of all you must fork this project into your GitHub account.

To create a fork on GitHub is as easy as clicking the “fork” button on the repository page.

<img src="https://docs.github.com/assets/images/help/repository/fork_button.jpg" alt="Fork on GitHub" width='450'>

### Installing

In this project you must use the VSCode SASS extension in order to compile SASS into CSS.

First of all you will need to install the extension:

- [Live SASS Compiler](https://marketplace.visualstudio.com/items?itemName=ritwickdey.live-sass)

When the extension is installed correctly, having a SASS file open, you must click on "Watch Sass":

<img src="https://raw.githubusercontent.com/ritwickdey/vscode-live-sass-compiler/master/images/Screenshot/AnimatedPreview.gif" width="600px">

If you want to change some configuration of "Live SASS Compiler" you can check this official resource:

- [Live SASS Compiler Settings](https://github.com/ritwickdey/vscode-live-sass-compiler/blob/master/docs/settings.md)

## Technologies used

\* SASS

\* CSS

\* HTML

## Project delivery

To deliver this project you must follow the steps indicated in the document:

- [Submitting a solution](https://www.notion.so/Submitting-a-solution-524dab1a71dd4b96903f26385e24cdb6)

## Resources

- [SASS documentation](https://sass-lang.com/)
- [W3S SASS](https://www.w3schools.com/sass/)
- [SASS Guidelines](https://sass-guidelin.es/es/)
- [Organizing SASS Projects](https://blog.prototypr.io/how-i-organize-sass-projects-e2d7760df86f)
- [Why don't use @import](https://www.youtube.com/watch?v=CR-a8upNjJ0)

#Questions
# Sass-proyect--clone-instagram

1.What is Sass?

Sass is a stylesheet language that’s compiled to CSS. It allows you to use variables, nested rules, mixins, functions, and more, all with a fully CSS-compatible syntax. Sass helps keep large stylesheets well-organized and makes it easy to share design within and across projects.

2.What does SASS stand for?
Syntactically awesome style sheets

3.What is a CSS pre-processor?
A computer program that modifies data to conform with the input requirements of another program.

4.What does a pre-processor have to do with SASS?
SCSS is a preprocessor which lets you use features that aren't a part of the wider CSS standard yet, and provides better workflows for maintaining your stylesheets. With SCSS preprocessor, you can reduce the amount of times you repeat yourself and ensure you're writing clean, maintainable code for the future.

5.Why use SASS?

Sass lets you use features that do not exist in CSS, like variables, nested rules, mixins, imports, inheritance, built-in functions, and other stuff.

6.SASS has disadvantages? Which are?

The developer must have enough time to learn new features present in this preprocessor before using it.
Using Sass may cause losing benefits of browser’s built-in element inspector.
Code has to be compiled
Dificult Troubleshooting

7.What is a SASS Variable? Explain why are useful

Just like other programming languages, Sass allows the use of variables that can store information you can use throughout your style sheet. For example, you can store a colour value in a variable at the top of the file, and then use this variable when setting the colour of your elements. This enables you to quickly change your colours without having to modify each line separately.

8.Explain the SASS variables property with an example.
Example:
    $font-stack:    Helvetica, sans-serif;
    $primary-color: #333;

body {
    font: 100% $font-stack;
    color: $primary-color;
}
9.What is a mixin? 

One of the advantages of using preprocessors is their ability to take complex, long-winded code and simplify it

9.1 Why is it important? Give an example

For example, if you need to include the vendor prefixes, you can use a mixin instead. Take a look at this example for border-radius:

@mixin border-radius($radius) {
    -webkit-border-radius: $radius;
    -moz-border-radius: $radius;
    -ms-border-radius: $radius;
    border-radius: $radius;
}

.box { @include border-radius(10px); }

Notice the @mixin directive at the top. It has been given the name border-radius and uses the variable $radius as its parameter. This variable is used to set the radius value for each element. 

10.What is SCSS? Give an example

The first, known as SCSS (Sassy CSS) and used throughout this reference, is an extension of the syntax of CSS. This means that every valid CSS stylesheet is a valid SCSS file with the same meaning. This syntax is enhanced with the Sass features described below. Files using this syntax have the .scss extension.

$color: red;

@mixin my-border($color) {
  border: 1px solid $color;
}

body {
  background: $color;
  @include my-border(green);
}

11.What is SASS? Give an example
provides a more concise way of writing CSS. It uses indentation rather than brackets to indicate nesting of selectors, and newlines rather than semicolons to separate properties. Files using this syntax have the .sass extension.

$color: red

=my-border($color)
  border: 1px solid $color

body
  background: $color
  +my-border(green)

12.What is the difference between .scss and .sass syntax.

Syntax is similar to CSS (so much that every regular valid CSS3 is also valid SCSS, but the relationship in the other direction obviously does not happen)

Uses braces {}
Uses semi-colons ;
Assignment sign is :
To create a mixin it uses the @mixin directive
To use mixin it precedes it with the @include directive
Files have the .scss extension.

Syntax is similar to Ruby
No braces
No strict indentation
No semi-colons
Assignment sign is = instead of :
To create a mixin it uses the = sign
To use mixin it precedes it with the + sign
Files have the .sass extension.
