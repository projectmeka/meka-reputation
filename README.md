# meka-reputation

## Purpose

This is a srml that used to calcuate user's `cross-chain reputation` based on the `cross-chain identity`([meka identity](https://github.com/projectmeka/meka-identity) and [meka passport](https://github.com/projectmeka/meka-passport))

Through bridge or Oracles, the blockchain can get user's cross-chain history transactions. Accorting to the rules of

This module is inclued in the [make-node](https://github.com/projectmeka/meka-node)

## Structure

### api(module)

### storage

### events

## Dependencies

### Traits

This module does not depend on any externally defined traits.

### Modules

This module does not depend on any other SRML or externally developed modules.

## Installation

### Runtime `Cargo.toml`

To add this module to your runtime, simply include the following to your runtime's `Cargo.toml` file:

```rust
[dependencies.substrate-module-template]
default_features = false
git = 'https://github.com/shawntabrizi/substrate-module-template.git'
```

and update your runtime's `std` feature to include this module:

```rust
std = [
    ...
    'example_module/std',
]
```

### Runtime `lib.rs`

You should implement it's trait like so:

```rust
/// Used for the module test_module
impl substrate_module_template::Trait for Runtime {
	type Event = Event;
}
```

and include it in your `construct_runtime!` macro:

```rust
ExampleModule: substrate_module_template::{Module, Call, Storage, Event<T>},
```

### Genesis Configuration

This template module does not have any genesis configuration.

## Reference Docs

You can view the reference docs for this module by running:

```
cargo doc --open
```

or by visiting this site: <Add Your Link>
