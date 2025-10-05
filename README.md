# macOS Tests

Please see ``preinstall.sh`` for installing prerequisites from the Anaconda Python distribution.

Please see ``travis_tests.sh`` for an example of how to setup and run the tests.

Results are sensitive to the CPU and system libraries that may be installed on your Mac OS X computer.

All tests pass on macOS Sequoia 15.7.1 on a Apple M2.

Trial run from a Anaconda Python environment:

```
source preinstall.sh
pip install --target devsim_macos_arm64_2.10.0 devsim-2.10.0-cp39-abi3-macosx_14_0_arm64.whl
chmod u+x devsim_macos_arm64_2.10.0/devsim_data/testing/rundifftest.py
bash travis_tests.sh 2.10.0
```
