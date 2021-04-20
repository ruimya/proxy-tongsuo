
# Envoy BabaSSL Extensions

The Envoy BabaSSL Extensions project hosts extensions for building
[Envoy](https://github.com/envoyproxy/envoy) purely with BabaSSL.

## Building

To build BabaSSL-enabled Envoy run the following command.

```console
$ bazel build //:envoy
```

If you need BabaSSL dynamically linked to Envoy then re-map `@boringssl` to
`@openssl_shared` by editing the [WORKSPACE](WORKSPACE) file.

## Testing

To test the BabaSSL features run the following commands.

```console
$ bazel test //test/common/...
$ bazel test //test/extensions/...
$ bazel test //test/integration/...
```

## License

The Envoy BabaSSL Extensions project is governed by the Apache License, Version
2.0. See the [LICENSE](LICENSE) file for the full license text.
