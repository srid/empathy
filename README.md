# empathy

[![Build Status](https://action-badges.now.sh/fused-effects/fused-effects)](https://github.com/fused-effects/fused-effects/actions) [![Hackage](https://img.shields.io/hackage/v/empathy.svg)](https://hackage.haskell.org/package/empathy)

`empathy` is a modern library for typed path manipulation. It takes advantage of newer GHC features like `DataKinds`, Backpack, and custom type errors so as to minimize the library footprint while yielding the maximum amount of type safety.

## Why not [one of the alternative typed-path libraries]?

I evaluated all of the libraries and wasn't happy with any of them. `pathtype` came closest to my needs, but bears historical cruft and doesn't take full advantage of newer GHC features. `path` requires Template Haskell and foregoes a rich path structure in favor of wrapping a bare string. `data-filepath` has a rich path structure but is unmaintained.

## This uses Backpack; does that mean it doesn't work with `stack`?

Alas, yes. Until https://github.com/commercialhaskell/stack/issues/2540 is fixed, you won't be able to use this library from a Stack project. (I should point out, however, that switching from `stack` to `cabal-install` v3.0 is generally pretty easy.)

# License

`empathy` is open-source software provided to you under the terms of the [Hippocratic License](https://firstdonoharm.dev). Due to the fact that the Hippocratic license does not have an SPDX identifier yet, the Cabal file states that it is MIT licensed; this will be addressed when the SPDX allocates an identifier for the HL.
