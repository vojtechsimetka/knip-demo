# knip-demo

Trying to get knip working with sveltekit. Running into following error

`npm run knip`

```sh
> knip-demo@0.0.1 knip
> knip

Analyzing workspace (.)...
file:///Users/redacted/knip-demo/node_modules/knip/dist/util/loader.js:28
        throw new LoaderError(`Error loading ${filePath}`, { cause: error });
              ^

LoaderError: Error loading /Users/redacted/knip-demo/vite.config.ts
    at load (file:///Users/redacted/knip-demo/node_modules/knip/dist/util/loader.js:28:15)
    at Module.findVitestDependencies (file:///Users/redacted/knip-demo/node_modules/knip/dist/plugins/vitest/index.js:10:26)
    at WorkspaceWorker.findDependenciesByPlugins (file:///Users/redacted/knip-demo/node_modules/knip/dist/workspace-worker.js:217:59)
    at processTicksAndRejections (node:internal/process/task_queues:96:5)
    at async WorkspaceWorker.findAllDependencies (file:///Users/redacted/knip-demo/node_modules/knip/dist/workspace-worker.js:236:9)
    at async main (file:///Users/redacted/knip-demo/node_modules/knip/dist/index.js:119:30)
    at async run (file:///Users/redacted/knip-demo/node_modules/knip/dist/cli.js:26:46)
    at async file:///Users/redacted/knip-demo/node_modules/knip/dist/cli.js:57:1 {
  [cause]: Error [ERR_PACKAGE_PATH_NOT_EXPORTED]: Package subpath './vite' is not defined by "exports" in /Users/redacted/knip-demo/node_modules/@sveltejs/kit/package.json
      at new NodeError (node:internal/errors:387:5)
      at throwExportsNotFound (node:internal/modules/esm/resolve:365:9)
      at packageExportsResolve (node:internal/modules/esm/resolve:589:7)
      at resolveExports (node:internal/modules/cjs/loader:554:36)
      at Function.Module._findPath (node:internal/modules/cjs/loader:594:31)
      at Function.Module._resolveFilename (node:internal/modules/cjs/loader:1007:27)
      at Function.resolve (node:internal/modules/cjs/helpers:114:19)
      at _resolve (/Users/redacted/knip-demo/node_modules/jiti/dist/jiti.js:1:241025)
      at jiti (/Users/redacted/knip-demo/node_modules/jiti/dist/jiti.js:1:243309)
      at /Users/redacted/knip-demo/vite.config.ts:1:175 {
    code: 'ERR_PACKAGE_PATH_NOT_EXPORTED'
  }
}

```
