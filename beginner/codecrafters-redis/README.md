# CodeCrafters - Build your own Redis

This is a starting point for Go solutions to the ["Build Your Own Redis" Challenge](https://codecrafters.io/challenges/redis)
([Starter](https://github.com/codecrafters-io/redis-starter-go), [Tester](https://github.com/codecrafters-io/redis-tester/)).

In this challenge, we'll build a toy Redis clone that's capable of handling basic commands like `PING`, `SET` and `GET`.
Along the way we'll learn about event loops, the Redis protocol and more.

## How to run locally

The entry point for the Redis implementation is in [`app/server.go`](./app/server.go).

If you're on Windows, you may have an issue with sh file permissions.
Run `git update-index --chmod=+x spawn_redis_server.sh` and `git config core.filemode false` to fix it.

Run `./spawn_redis_server.sh` to run your Redis server.

From another terminal, test it with `telnet localhost 6379` then send commands (enter `close` to exit).
