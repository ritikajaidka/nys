## `process.env`

The `process.env` property returns an object containing the user environment.

## `dotenv` 

Which is a zero-dependency module that loads environment variables from a .env file into process.env. Storing configuration in the environment separate from code
```bash
~source https://www.npmjs.com/package/dotenv 
```
### PORT
We are getting port from config file. In case, config port is not available, `port3000` will come into action.

```jsx
const port = process.env.PORT || 3000;
``` 

```bash
{
  TERM: 'xterm-256color',
  SHELL: '/usr/local/bin/bash',
  USER: 'maciej',
  PATH: '~/.bin/:/usr/bin:/bin:/usr/sbin:/sbin:/usr/local/bin',
  PWD: '/Users/maciej',
  EDITOR: 'vim',
  SHLVL: '1',
  HOME: '/Users/maciej',
  LOGNAME: 'maciej',
  TERM_PROGRAM: 'vscode',
  NODE: '/usr/local/bin/node',
  INIT_CWD: '/Users/myuser/gitStore/nys',
  SHELL: '/bin/zsh',
  TERM: 'xterm-256color',
  npm_config_metrics_registry: 'https://registry.npmjs.org/',
  TMPDIR: '/var/folders/7h/j8p2tc210sl2hjcwm7t4zq2c0000gn/T/',
  npm_config_global_prefix: '/usr/local',
  TERM_PROGRAM_VERSION: '1.71.0',
  ZDOTDIR: '/var/folders/7h/j8p2tc210sl2hjcwm7t4zq2c0000gn/T/vscode-zsh',
  ORIGINAL_XDG_CURRENT_DESKTOP: 'undefined',
  MallocNanoZone: '0',
  COLOR: '1',
  TERM_SESSION_ID: '008D8FDA-7226-44D0-B9CC-07CDEAA6A731',
  npm_config_noproxy: '',
  EDITOR: 'vi',
  npm_package_name: 'nys',
  LANG: 'en_US.UTF-8',
  VSCODE_GIT_ASKPASS_EXTRA_ARGS: '--ms-enable-electron-run-as-node',
  XPC_FLAGS: '0x0',
  npm_config_node_gyp: '/usr/local/lib/node_modules/npm/node_modules/node-gyp/bin/node-gyp.js',
  npm_package_version: '1.0.0',
  XPC_SERVICE_NAME: '0',
  VSCODE_INJECTION: '1'
}
```

## `app.listen`

Binds and listens for connections on the specified host and port.

```
const server = app.listen(port, () => {
  console.log(`App running on port ${port}...`);
});
```