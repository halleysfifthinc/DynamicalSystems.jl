# v0.3.0:
* Added method to estimate optimal delay time `estimate_delay`.
* Added abstract `AbstractDataset` supertype.
* Completely changed the way `Reconstruction` is done.
* Added more methods, interaction and smart indexing related to the (new)
  `Reconstruction` object. See the new docstring of `reconstruct` for usage.
* Added a new method that enables the calculation of the maximum Lyapunov
  exponent from a numeric timeseries (like an experimental recording).
  This method (called `numericallyapunov`) operates on a reconstruction, **using
  4 different algorithms**. See the docstring of `numericallyapunov` for
  more info!
* Added `double_pendulum` to famous systems.

# v0.2.0: Major Improvements and new features
+ Improved algorithm for deducing best boxsizes (using `min_pairwise_distance`)
+ All numerical data is now structured and expected to be in the `Dataset` Type,
  which by itself defines a new interface (identical to matrix).
+ Major speed improvements in lyapunov function calculation.
+ Major speed improvements in histogram computation.
+ A new qr method for small matrices, faster than `Base.qr` (see `qr_sq`).
+ Reconstruction interface.
+ New and better docs.
+ Better integration of `SVectors` in the package all around.
+ Better default keywords for attractor dimension and lyapunov exponents.
+ Equations of motion on all famous systems.

# v0.1.0: First release
Normal changelog will be kept from this point onwards.
