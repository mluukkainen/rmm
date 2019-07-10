# RMM 0.8.0 (Date TBD)

## New Features

    - PR #95 Add skip test functionality to build.sh
    - PR #103 force running tests, does branch-0.9 testing work

## Improvements

    ...

## Bug Fixes

 - PR #92 Update docs version


# RMM 0.7.0 (10 May 2019)

## New Features

 - PR #67 Add random_allocate microbenchmark in tests/performance
 - PR #70 Create conda environments and conda recipes
 - PR #77 Add local build script to mimic gpuCI
 - PR #80 Add build script for docs

## Improvements

- PR #76 Add cudatoolkit conda dependency
- PR #84 Use latest release version in update-version CI script
- PR #90 Avoid using c++14 auto return type for thrust_rmm_allocator.h 

## Bug Fixes

 - PR #68 Fix signed/unsigned mismatch in random_allocate benchmark
 - PR #74 Fix rmm conda recipe librmm version pinning
 - PR #72 Remove unnecessary _BSD_SOURCE define in random_allocate.cpp


# RMM 0.6.0 (18 Mar 2019)

## New Features

 - PR #43 Add gpuCI build & test scripts
 - PR #44 Added API to query whether RMM is initialized and with what options.
 - PR #60 Default to CXX11_ABI=ON

## Improvements

## Bug Fixes

 - PR #58 Eliminate unreliable check for change in available memory in test
 - PR #49 Fix pep8 style errors detected by flake8


# RMM 0.5.0 (28 Jan 2019)

## New Features

 - PR #2 Added CUDA Managed Memory allocation mode

## Improvements

 - PR #12 Enable building RMM as a submodule
 - PR #13 CMake: Added CXX11ABI option and removed Travis references
 - PR #16 CMake: Added PARALLEL_LEVEL environment variable handling for GTest build parallelism (matches cuDF)
 - PR #17 Update README with v0.5 changes including Managed Memory support

## Bug Fixes

 - PR #10 Change cnmem submodule URL to use https
 - PR #15 Temporarily disable hanging AllocateTB test for managed memory
 - PR #28 Fix invalid reference to local stack variable in `rmm::exec_policy`


# RMM 0.4.0 (20 Dec 2018)

## New Features

- PR #1 Spun off RMM from cuDF into its own repository.

## Improvements

- CUDF PR #472 RMM: Created centralized rmm::device_vector alias and rmm::exec_policy
- CUDF PR #465 Added templated C++ API for RMM to avoid explicit cast to `void**`

## Bug Fixes


RMM was initially implemented as part of cuDF, so we include the relevant changelog history below.

# cuDF 0.3.0 (23 Nov 2018)

## New Features

 - PR #336 CSV Reader string support

## Improvements

 - CUDF PR #333 Add Rapids Memory Manager documentation
 - CUDF PR #321 Rapids Memory Manager adds file/line location logging and convenience macros

## Bug Fixes


# cuDF 0.2.0 and cuDF 0.1.0

These were initial releases of cuDF based on previously separate pyGDF and libGDF libraries. RMM was initially implemented as part of libGDF.

