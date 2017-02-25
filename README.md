# Node.js + Xvfb

This is a Dockerfile (and Docker image) for Node.js and Xvfb. Useful for virtual browser testing with Node.js. This can be used with node modules that use [Electron](http://ghub.io/electron), such as [browser-run](http://ghub.io/browser-run) and [tape-run](http://ghub.io/tape-run).

Before you can use this, you will need to start a xvfb server. Something like this should work:

```bash
export DISPLAY=:9.0
Xvfb -ac -screen scrn 1024x768x24 :9.0 &
```
