# Pay it Forward
[![Build Status](//img.shields.io/travis/asm-products/pay-it-forward/develop.svg)](//travis-ci.org/asm-products/pay-it-forward)
[![Code Climate](//img.shields.io/codeclimate/github/asm-products/pay-it-forward.svg)](//codeclimate.com/github/asm-products/pay-it-forward)
[![Coverage Status](//img.shields.io/coveralls/asm-products/pay-it-forward/develop.svg)](//coveralls.io/r/asm-products/pay-it-forward?branch=develop)
[![Dependency Status](//img.shields.io/gemnasium/asm-products/pay-it-forward.svg)](//gemnasium.com/asm-products/pay-it-forward)
[![Security Status](//hakiri.io/github/asm-products/pay-it-forward/develop.svg)](//hakiri.io/github/asm-products/pay-it-forward/develop)


## Built With
Open Source:
- [Ruby on Rails](//github.com/rails/rails)
- [PostgreSQL](//www.postgresql.org/)
- [jQuery](//jquery.com/)
- [Bootstrap](//github.com/twbs/bootstrap)

Services:
- [Heroku](//www.heroku.com/)
- [S3](//aws.amazon.com/s3/)

## Setup
#### Setup Backing Resources
- [Setup Postgres](//wiki.postgresql.org/wiki/Detailed_installation_guides)
- Run `./bin/setup`
  - If you run into any error, configure the `.env` file and retry.


#### Environment Variables
- All
  - `DATABASE_URL`: _`postgresql://username:password@host:port/database`_

- Development
  - `TRUSTED_IP`: _`172.17.42.1`_ ([Better Errors](//github.com/charliesome/better_errors): [Optional](//github.com/charliesome/better_errors#security))

- Production
  - `APP_HOST`: _`example.com`_
  - `SECRET_KEY_BASE`: _`ea1e8ba83614cc8d6140105a42642dc8391d6f2f8...`_
  - `SECRET_KEY_DEVISE`: _`5c38552c853e969d026794035f8f1953032d60bc...`_
  - `DEVISE_PEPPER`: _`2ae31cfd67205ceba77c4ebe501651de78e68d7d...`_
  
  - [Twitter](//apps.twitter.com/)
    - `TWITTER_KEY`: _`lkfAc16oTJcbR766zw8GDw...`_
    - `TWITTER_SECRET`: _`NT7WOYKnZplMYQeJ8GjeXHup9sPk5WbR1WZFritdnARP5x7...`_
  
  - [Facebook](//developers.facebook.com)
    - `FACEBOOK_KEY`: _`559887567744...`_
    - `FACEBOOK_SECRET`: _`445a594f443e2f1bcd3025f99e693...`_
  
  - [AWS](//aws.amazon.com/)
    - `AWS_ACCESS_KEY_ID`: _`AKIAIOSFODNN7EXAM...`_ 
    - `AWS_SECRET_ACCESS_KEY`: _`wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLE...`_
    - `AWS_S3_REGION`: _`us-east-1`_
    - `AWS_S3_BUCKET`: _`name`_
    - `AWS_S3_FQDN`: _`//localhost`_
    - `ASSETS_DIRECTORY`: _`/development/assets`_
  
  - [Stripe](//stripe.com/)
    - `STRIPE_KEY`: _`sk_test_4TYeUPbdKFGeJUXBVJFoI...`_


## Contributing
This project's git flow is based on [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)

1. Find or Submit Bounty
2. Make a Feature Branch from `develop`
  - Name it based on bounty: `18-init-project`
3. Make Changes
  - Use micro commits
  - Use the imperative, present tense: "change", not "changed" or "changes".
4. Write tests
  - Will not accept PRs that reduce coverage
5. Open PR back into develop
  - Make PR Description links to the Bounty and add a comment to the Bounty linking the PR
  - Add accompanying images for UI changes
