# Spin gRPC RouteGuide Example

This example is adapted from [`routeguide`](TODO) example in the [`tonic`](TODO) repository to run in a Spin application.

The current example includes an example for making a unary and uni-direction streaming gRPC requests.

To test, start the routeguide-server from the tonic repository:

```console
$ cargo run --bin routeguide-server
...
RouteGuideServer listening on: [::1]:10000
```

In another terminal, build and run the example:
```
$ spin up --build
```

In another terminal, send a request:
```console
$ curl localhost:3000/get_feature
Feature: Feature { name: "Berkshire Valley Management Area Trail, Jefferson, NJ, USA", location: Some(Point { latitude: 409146138, longitude: -746188906 }) }