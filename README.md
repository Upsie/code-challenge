# upsie interview challenge

# Hello!

Thanks for applying to Upsie! We have a 2 part code challenge for you to work on during this interview. Our primary goal here is not to necessarily land on a final solution but to see how you approach solving problems and how well you communicate around that process. Our secondary goal is to evaluate your eye for aesthetics and UI layout.

We want this to be as real world as possible so feel free to use the internet just like you would normally. Don't feel like you have to show off a fancy algorithm just because. we are a startup and that's about getting things done quickly in as reliable a way possible. The more we can be forward looking and not spending time fixing prior work, the better.

# The Challenge

## context

A fictitious company stores a list of software products they use. They have stored the name, version, an icon for, and description of each product. They have asked us to create a simple website where users can type in a version number and receive a list of software products that are greater than the version they entered and then see some basic information about the resulting software titles.

The software versions are stored as a string in [semantic versioning](https://semver.org/) format [major version].[minor version].[patch]. You may see versions like “2”, “1.5”, or “2.12.4” (these are all valid inputs from the user as well). The period is only used as a separator and does not represent a decimal point – 1.5 does not mean one and a half.

"2" == "2.0" == "2.0.0"
"2" < "2.0.1"
"2" < "2.1"
"2.0.1" < "2.1.0"

The list of software has been provided in JSON format below but feel free to adapt the format of this list as desired to easily drop into your overall solution. This site will be publicly available, so user authentication will not be required.

## todays objective

There are two core components to this challenge.

1. filtering the software list
2. displaying the software list

For the sake of time, we'd like to whiteboard and/or psuedo code part 1, and then work up a prototype for part 2.

# Software Product List

```json
[
  {
    "name": "MS Word",
    "version": "13.2.1.",
    "icon": "file-word",
    "description": "Use Microsoft Word for the best word processing and document creation. Find out how document collaboration and editing tools can help polish your Word docs"
  },
  {
    "name": "MS Excel",
    "version": "13.4.2",
    "icon": "file-excel",
    "description": "Microsoft Excel is the industry leading spreadsheet program, a powerful data visualization and analysis tool. Take your analytics to the next level with Excel."
  },
  {
    "name": "AngularJS",
    "version": "1.7.1",
    "icon": "angular",
    "description": "HTML is great for declaring static documents, but it falters when we try to use it for declaring dynamic views in web-applications. AngularJS lets you extend HTML vocabulary for your application. The resulting environment is extraordinarily expressive, readable, and quick to develop."
  },
  {
    "name": "Angular",
    "version": "8.1.13",
    "icon": "angular",
    "description": "HTML is great for declaring static documents, but it falters when we try to use it for declaring dynamic views in web-applications. AngularJS lets you extend HTML vocabulary for your application. The resulting environment is extraordinarily expressive, readable, and quick to develop."
  },
  {
    "name": "React",
    "version": "0.0.5",
    "icon": "react",
    "description": "A JavaScript library for building user interfaces"
  },
  {
    "name": "Vue.js",
    "version": "2.6",
    "icon": "vuejs",
    "description": "The Progressive JavaScript Framework."
  },
  {
    "name": "Ember.js",
    "version": "3.10.1",
    "icon": "ember",
    "description": "Ember.js helps developers be more productive out of the box. Designed with developer ergonomics in mind, its friendly APIs help you get your job done—fast."
  },
  {
    "name": "Visual Studio Code",
    "version": "1.39.2",
    "icon": "code",
    "description": "Visual Studio Code is a code editor redefined and optimized for building and debugging modern web and cloud applications.  Visual Studio Code is free and available on your favorite platform - Linux, macOS, and Windows."
  },
  {
    "name": "Atom",
    "version": "1.41.0",
    "icon": "atom",
    "description": "At GitHub, we’re building the text editor we’ve always wanted: hackable to the core, but approachable on the first day without ever touching a config file. We can’t wait to see what you build with it."
  },
  {
    "name": "Sublime",
    "version": "3.12.0",
    "icon": "",
    "description": "Sublime Text is a sophisticated text editor for code, markup and prose. You'll love the slick user interface, extraordinary features and amazing performance."
  },
  {
    "name": "DataGrip",
    "version": "2019.2.6",
    "icon": "",
    "description": "Enjoy working with databases · Intelligent query console · Efficient schema navigation · Explain plan · Smart code completion · On-the-fly analysis and quick-fixes."
  }
]
```
