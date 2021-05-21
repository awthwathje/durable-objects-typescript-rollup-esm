# Durable Objects TypeScript Counter template

## NOTE: You must be using wrangler 1.16.0-durable-objects.rc.0 or newer to use this template

A template for kick starting a Cloudflare Workers project using:

- Durable Objects
- TypeScript
- Jest for unit testing
- Modules (ES Modules to be specific)
- Rollup
- Wrangler

Worker code is in `src/`. The Durable Object `CounterTs` class is in `src/counter.ts`, and the eyeball script is in `index.ts`.

Rollup is configured to output a bundled ES Module to `dist/index.mjs`.

There's an example unit test in `src/index.test.ts`, which will run as part of `wrangler build`.   To run tests on their own use `npm test`.

On your first publish, you must use `wrangler publish --new-class CounterTs` to allow the CounterTs class to implement Durable Objects.
