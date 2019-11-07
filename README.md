# Hello!

Thanks for applying to Upsie! We have a code challenge for you to complete ahead of your interview. We’ll review it and use it as a source of conversation about coding, so please be prepared to talk about your solution, why you approached the problem the way you did and how you might have done it differently.

Our goal here is to allow you to write code in a low stress environment on your own computer in a language and/or framework you're familiar with. We realize we’re asking you to do on your own time, but we prefer this format over a long session of whiteboarding code in an interview.

Try not to spend more than 4 hours on this challenge. If you reach the 4-hour mark and are not finished, just turn it in as-is and let us know what you would have done with more time.

# The Challenge

An fictitious company stores a list of software products they use. They have stored the name and version of each product. They have asked us to create a simple website where users can type in a version number and receive a list of software products that are greater than the version they entered.

The software versions are stored as a string in the format [major version].[minor version].[patch]. You may see versions like “2”, “1.5”, or “2.12.4” (these are all valid inputs from the user as well). The period is only used as a separator and does not represent a decimal point – 1.5 does not mean one and a half.

"2" == "2.0" == "2.0.0"
"2" < "2.0.1"
"2" < "2.1"
"2.0.1" < "2.1.0"

The list of software has been provided in JSON format below but feel free to adapt the format of this list as desired to easily drop into your overall solution.

This site will be publicly available, so user authentication will not be required.

# Software Product List

```json
[
  {
    "name": "MS Word",
    "version": "13.2.1."
  },
  {
    "name": "MS Excel",
    "version": "13.4.2"
  },
  {
    "name": "AngularJS",
    "version": "1.7.1"
  },
  {
    "name": "Angular",
    "version": "8.1.13"
  },
  {
    "name": "React",
    "version": "0.0.5"
  },
  {
    "name": "Vue.js",
    "version": "2.6"
  },
  {
    "name": "Ember.js",
    "version": "3.10.1"
  },
  {
    "name": "Visual Studio Code",
    "version": "1.39.2"
  },
  {
    "name": "Atom",
    "version": "1.41.0"
  },
  {
    "name": "Sublime",
    "version": "3.12.0"
  },
  {
    "name": "DataGrip",
    "version": "2019.2.6"
  }
]
```
