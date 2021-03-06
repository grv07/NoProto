# 0.6.1 December 15, 2020
- Restored the first byte for later use.  Probably add `u32` address size again in the future.
- The format should now be considered stable, won't be making any further changes to it.
- Removed all panics, unwraps, and `unreachable_unchecked` calls.
- Strings now support `lowercase` and `uppercase` properties in schema.
- Added sortable buffer export and import capability.
- Cleaned up benchmark formatting a bit.

# 0.6.0 December 14, 2020
- Complete rewrite again (twice this time).
- There is now only one address size, `u16`, limits buffers to 16kb max size.
- Dramatically reduced the cost of reading/updating addresses in buffer.
- Lists & maps are now limited to 255 items.
- Performance is now comparable to Protocol Buffers, I'm pretty happy about that.

# 0.5.1 November 30, 2020
- Forgot to apply `no_std` after debugging in previous release.

# 0.5.0 November 30, 2020
- Complete rewrite with major performance improvements.
- Optimizations and cleaning code.
- More documentation, less noise.
- 10 - 15x performance improvements on data inserts

# 0.4.2 November 20, 2020
- Optimizations and cleaning code.
- More documentation, less noise.

# 0.4.1 November 19, 2020
- Docs & Meta update

# 0.4.0 November 19, 2020
- Completely reworked loop code for all collections, it's now far faster and more efficient.
- Iterating/Traversing over a buffer no longer mutates it.
- Added new `to_iter` and `list_push` methods to buffer.
- Removed `open` and `extract` methods from buffer, you can no longer access internal pointers directly.
- Several other minor optimizations.

# 0.3.0 November 11, 2020
- Added lots of tests
- Reorganized files a little bit.
- Byte schemas are now parsed ahead of time instead of incrementally
- Slight adjustment to the schema byte format.
- Tuple sorting validation is now more thorough
- Cleaned up lots of code.

# 0.2.2 November 10, 2020
- Added lots of tests and documentation.
- Removed all Rc's from the library.
- Added compiled byte schemas & format docs with tests.

# 0.1.2 August 26, 2020
- Added lots of tests, fixed a few small bugs.
- Added some info to README.

# 0.1.1 August 26, 2020
- Added data format documentation.

# 0.1.0 August 26, 2020
- Stabilized API
- Added macro for numbers data type
- Minor optimizations