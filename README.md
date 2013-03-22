# summerofdrones.com

The [summerofdrones.com](summerofdrones.com ) website.

## Setup

Clone the repo, then install the following gems:

```
gem install jekyll -v 1.0.0.beta2
gem install jekyll-less
```

You can now run the site locally on port 400 using:

```bash
$ jekyll server
```

## Deployment

The site is deployed to s3. The credentials are in the credentials repo.

Going forward, I'll also setup a CI server to deploy every commit to master.
