[![CI](https://github.com/18F/api.data.gov/workflows/CI/badge.svg)](https://github.com/18F/api.data.gov/actions?workflow=CI) [![Code Climate](https://codeclimate.com/github/18F/api.data.gov/badges/gpa.svg)](https://codeclimate.com/github/18F/api.data.gov) [![Known Vulnerabilities](https://snyk.io/test/github/18F/api.data.gov/badge.svg?targetFile=Gemfile.lock)](https://snyk.io/test/github/18F/api.data.gov?targetFile=Gemfile.lock) [![Known Vulnerabilities](https://snyk.io/test/github/18F/api.data.gov/badge.svg?targetFile=requirements.txt)](https://snyk.io/test/github/18F/api.data.gov?targetFile=requirements.txt)

# api.data.gov

[https://api.data.gov](https://api.data.gov/) is a free API management service for federal agencies. Our aim is to make it easier for agencies to release and manage APIs. You can sign up for a single API key and use it across participating government services [here](https://api.data.gov/signup/). You can also find our documentation [here](http://api.data.gov/docs/).



* [Program Notes for api.data.gov](https://github.com/18F/api.data.gov/wiki/Program-Notes)
* [GitHub Repository for API Umbrella](https://github.com/NREL/api-umbrella), the underlying technology of `api.data.gov`

## Notes 

To edit this site, edit the `Master` branch.  Changes should take effect within minutes.  

The website content for api.data.gov built with [Middleman](http://middlemanapp.com).

All contributions are welcome. To submit a change, fork this repo, commit your changes, and send us a [pull request](https://help.github.com/articles/using-pull-requests).

To edit the agency list on the homepage, create or edit [a page like this](https://github.com/18F/api.data.gov/blob/main/source/docs/fda.md) for each agency.


## Setup

Ruby 1.9+ is required to build the site.

```sh
$ git submodule update --init --recursive # Make sure to pull in git submodules
$ gem install bundler
$ bundle install --binstubs
```

## Development

The content files to edit are in `./source`. You can view your changes as you make them by running the Middleman preview server:

```sh
$ ./bin/middleman server
```

This will start a local web server running at [http://localhost:4567/](http://localhost:4567/)

After you're happy with your changes, commit and submit a pull request.

## Deploy

To publish to production with GitHub Pages:

```sh
$ ./bin/rake publish
```


### Public domain

This project is in the worldwide [public domain](LICENSE.md). As stated in [CONTRIBUTING](CONTRIBUTING.md):

> This project is in the public domain within the United States, and copyright and related rights in the work worldwide are waived through the [CC0 1.0 Universal public domain dedication](https://creativecommons.org/publicdomain/zero/1.0/).
>
> All contributions to this project will be released under the CC0 dedication. By submitting a pull request, you are agreeing to comply with this waiver of copyright interest.
