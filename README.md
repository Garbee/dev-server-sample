# Steps to reproduce

1. Clone repo
2. Run `npm ci`
3. Run `npm run serve`
4. Observe console in terminal of browser tab

You'll see "Unexpected EOF".

When running through @web/dev-server, the file is being mutated it seems to have the last quote removed.

It is valid syntax in the [upstream package](https://www.npmjs.com/package/@langchain/core?activeTab=code).
Navigate to `runnables/remote.js` to confirm.
