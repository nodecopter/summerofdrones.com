# summerofdrones.com

The [summerofdrones.com](summerofdrones.com ) website.

## Setup

Clone the repo, then install the following gems:

``` sh
gem install bundler
cd summerofdrones.com
bundle install
```

You can now run the site locally on port 4000 using:

```bash
jekyll --auto --server
```

## Deployment

The site is deployed with
[jekyll-s3](https://github.com/laurilehmijoki/jekyll-s3). The credentials are
in the credentials repo.

Going forward, I'll also setup a CI server to deploy every commit to master.
