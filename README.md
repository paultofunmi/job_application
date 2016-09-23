Job Assessment Project
===============

---

#### This sample exercise was built using GOV.UK elements[https://github.com/alphagov/govuk_elements] and other dependencies such as govuk_frontend_toolkit[https://github.com/alphagov/govuk_frontend_toolkit], 
 and GOV.UK template[https://github.com/alphagov/govuk_template]

---

## What is it?

Job Assessment Project:

1. [an online design guide](http://govuk-elements.herokuapp.com/), explaining how to make your service look consistent with the rest of GOV.UK
2. an example of how to use the code in the [GOV.UK template](https://github.com/alphagov/govuk_template) and the [GOV.UK frontend toolkit](https://github.com/alphagov/govuk_frontend_toolkit)
3. an [npm package of the Sass files](https://www.npmjs.com/package/govuk-elements-sass)

The guide can be seen here: [http://govuk-elements.herokuapp.com](http://govuk-elements.herokuapp.com/).



## Installation guide(To run this nodeJS application)

To install the jobassessment on your local machine, you need node package manager. The steps are:

 Install the required node modules

    npm install


  Run the app

    npm start

Go to [localhost:3000](http://localhost:3000) in your browser.


## Testing the app

### GOV.UK lint
[GOV.UK elements uses govuk-lint](https://github.com/alphagov/govuk-lint#sass), which uses [scss-lint](https://github.com/brigade/scss-lint) as its scss linter.

### Standard JavaScript
GOV.UK elements uses [standardjs](http://standardjs.com/), an opinionated JavaScript linter. All JavaScript files follow its conventions.

Both linters run on CI to ensure that new pull requests are in line with them.

## Linting

To check the whole codebase, run:

    npm test

## Running Wraith to compare changes

GOV.UK elements uses Wraith so that regressions can be easily spotted.

This needs to be run from the Wraith directory `/tests/wraith` and some dependencies need to be installed on the local machine first.

### Install Wraith and its dependencies

    gem install wraith
    brew install phantomjs
    brew install imagemagick

### Usage

Take a baseline of the current version.
On master run:

    wraith history config.yaml


Switch to your feature branch and make changes.
On feature branch run:

    wraith latest config.yaml




