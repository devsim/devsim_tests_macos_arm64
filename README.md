# macOS Tests

Please see ``preinstall.sh`` for installing prerequisites from the Anaconda Python distribution.

Please see ``travis_tests.sh`` for an example of how to setup and run the tests.

Results are sensitive to the CPU and system libraries that may be installed on your Mac OS X computer.

All tests pass on macOS Sonoma 14.6.1 on a Apple M2.

Trial run from a Anaconda Python environment:

```
source preinstall.sh
pip install --target devsim_macos_arm64_2.9.0 devsim-2.9.0-cp37-abi3-macosx_12_0_universal2.whl
chmod u+x devsim_macos_arm64_2.9.0/devsim_data/testing/rundifftest.py
bash travis_tests.sh 2.9.0
```
