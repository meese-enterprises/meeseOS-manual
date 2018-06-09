# Settings Guide

OS.js provides options for customizing the settings storage.

Two dapters are provided by default:

* `server`
* `localStorage` (default)

## Configuring adapter

See [official resource list](/resource/official/README.md) for provided adapter.

> The README file of the module should provide more spesific exaples.

### Client

```javascript
core.register(SettingsServiceProvider, {
  args: {
    adapter: 'server'
  }
});
```

### Server

```javascript
core.register(SettingsServiceProvider, {
  args: {
    adapter: fn
  }
});
```

## Configuring defaults

The default settings are located in `@osjs/client/src/config.js`.