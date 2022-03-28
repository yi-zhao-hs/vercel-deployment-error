how to reproduce

1. run `vercel`

```
❯ vercel --debug
Vercel CLI 24.0.1
> [debug] [2022-03-28T13:34:52.784Z] user supplied no target, defaulting to deploy
> [debug] [2022-03-28T13:34:52.868Z] Spinner stopped (Retrieving project…)
> [debug] [2022-03-28T13:34:52.868Z] Spinner invoked (Retrieving project…) with a 1000ms delay
> [debug] [2022-03-28T13:34:52.896Z] #1 → GET https://api.vercel.com/teams/team_LZNJ8aR60nuwY5P1uj75ZoCu?teamId=team_LZNJ8aR60nuwY5P1uj75ZoCu
> [debug] [2022-03-28T13:34:52.899Z] #2 → GET https://api.vercel.com/projects/prj_gUBzVgrlEGJmvLdLY1i8EYtNlJ3G?teamId=team_LZNJ8aR60nuwY5P1uj75ZoCu
> [debug] [2022-03-28T13:34:53.172Z] #1 ← 200 OK: sfo1::rl6qd-1648474493238-1f2b837d45be [276ms]
> [debug] [2022-03-28T13:34:53.204Z] #2 ← 200 OK: sfo1::rl6qd-1648474493242-7fa6ba03de50 [305ms]
> [debug] [2022-03-28T13:34:53.223Z] Spinner stopped (Deploying hootsuite/website)
> [debug] [2022-03-28T13:34:53.223Z] Spinner invoked (Deploying hootsuite/website) with a 0ms delay
[client-debug] 2022-03-28T13:34:53.224Z Creating deployment...
[client-debug] 2022-03-28T13:34:53.225Z Provided 'path' is a directory.
[client-debug] 2022-03-28T13:34:53.238Z Found 25 rules in .vercelignore
[client-debug] 2022-03-28T13:34:53.238Z Building file tree...
[client-debug] 2022-03-28T13:34:53.242Z Found 0 files in the specified directory
[client-debug] 2022-03-28T13:34:53.243Z Deployment path has no files. Yielding a warning event
[client-debug] 2022-03-28T13:34:53.243Z Yielding a 'hashes-calculated' event with 0 hashes
[client-debug] 2022-03-28T13:34:53.244Z Using provided API URL: https://api.vercel.com
[client-debug] 2022-03-28T13:34:53.244Z Using provided user agent: vercel 24.0.1 node-v16.2.0 darwin (x64)
[client-debug] 2022-03-28T13:34:53.244Z Setting platform version to harcoded value 2
[client-debug] 2022-03-28T13:34:53.244Z Creating the deployment and starting upload...
[client-debug] 2022-03-28T13:34:53.244Z Determining necessary files for upload...
[client-debug] 2022-03-28T13:34:53.245Z Creating deployment
[client-debug] 2022-03-28T13:34:53.245Z Sending deployment creation API request
[client-debug] 2022-03-28T13:35:00.357Z Deployment response: {"error":{"code":"internal_server_error","message":"An unexpected internal error occurred"}}
[client-debug] 2022-03-28T13:35:00.357Z Error: Deployment request status is 500
[client-debug] 2022-03-28T13:35:00.357Z Yielding a 'error' event
> [debug] [2022-03-28T13:35:00.403Z] Error: Error: An unexpected internal error occurred
Error: An unexpected internal error occurred
    at Now.handleDeploymentError (/Users/yi.zhao/.local/share/nvm/v16.2.0/lib/node_modules/vercel/dist/index.js:240226:16)
    at Object.processDeployment [as default] (/Users/yi.zhao/.local/share/nvm/v16.2.0/lib/node_modules/vercel/dist/index.js:233441:41)
    at processTicksAndRejections (node:internal/process/task_queues:96:5)
    at Now.create (/Users/yi.zhao/.local/share/nvm/v16.2.0/lib/node_modules/vercel/dist/index.js:240110:28)
    at Object.createDeploy [as default] (/Users/yi.zhao/.local/share/nvm/v16.2.0/lib/node_modules/vercel/dist/index.js:233050:16)
    at module.exports.__webpack_modules__.28640.exports.default (/Users/yi.zhao/.local/share/nvm/v16.2.0/lib/node_modules/vercel/dist/index.js:225821:22)
    at main (/Users/yi.zhao/.local/share/nvm/v16.2.0/lib/node_modules/vercel/dist/index.js:231460:20)
Error! An unexpected internal error occurred
```