

### 2.0.5 - 2022-05-26

- fix: backwards compatibility with legacy plugin config files
- fix: rename p\* methods -> * (required in redis v4)
- fix: add `await client.connect()` as is now required, fixes #32
- fix: make redis_ping async
- dep(redis): bump 4.0 -> 4.1
- chore(ci): updated syntax
- chore(ci): added codeql config
- test: added tests for init_redis_plugin


### 2.0.0 - 2022-03-29

- dep(redis): bump major version 3 -> 4
- breaking API change: replaced callbacks with promises
- config.ini
    - opts.db -> opts.database (to match upstream)


### 1.0.13 - 2021-10-14

- chore(ci): switch CI from Travis to GitHub Actions
- doc(README): update formatting with GFM


### 1.0.12 - 2020-03-16

- chore(ci): replace nodeunit with mocha
- dep(redis): update lib to v3
- appveyor: test on node 10


### 1.0.11 - 2019-04-11

- create custom connection only after: all 3 conditions match


### 1.0.10 - 2019-04-09

- merge ALL of [opts] into [server] config (fixes #18)
- merge all of [opts] into [pubsub] config
- include an empty config/redis.ini
- add defaultOpts once, vs defaults in two places


### 1.0.9 - 2019-02-19

- bump redis version to 2.8.0
- emit error message if redis connection fails
- add 3s timeout for subscribe connects: minimize connections stalls
- add es6 template literals


### 1.0.8 - 2018-01-03

- upon punsubscribe, `quit()` (disconnect) redis client


### 1.0.7 - 2017-07-31

- apply config [opts] to pubsub settings #7


### 1.0.6 - 2017-06-16

- eslint 4 compat


### 1.0.5 - 2017-06-09

- disconnect per-connection redis client upon punsubscribe


### 1.0.4 - 2017-02-06

- remove retry_strategy, redis client now does The Right Thing w/o it


### 1.0.3 - 2017-02-06

- don't break when no [redis] config exists

