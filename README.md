This is a fork from [wilix-team/iohook](https://github.com/wilix-team/iohook). Since it no longer provides prebuild binary for new version Node.js and Electron, and not support Apple m1 (a.k.a amd64, aarch64), so I forked the project, provided prebuild binary files (based on iohook v0.9.3) and posted it to npm.

Just install it and it should work for you:

```text
npm install @hcfy/iohook
```

Use `arm64` in `package.json` runtime version to download arm64 prebuild.

[https://wilix-team.github.io/iohook/usage.html#electron](https://wilix-team.github.io/iohook/usage.html#electron)

For example, for Electron v17 and Node.js v16:

```js
"iohook": {
  "targets": [
    "node-93",
    "electron-101"
  ],
  "platforms": [
    "win32",
    "darwin",
    "linux"
  ],
  "arches": [
    "x64",
    "ia32",
    "arm64"
  ]
}
```