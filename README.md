# macOS Tests

Please see ``preinstall.sh`` for installing prerequisites from the Anaconda Python distribution.

Please see ``travis_tests.sh`` for an example of how to setup and run the tests.

Results are sensitive to the CPU and system libraries that may be installed on your Mac OS X computer.

All tests pass on macOS Sonoma 14.5 on a Mac mini M1, 2020.

Trial run from a Anaconda Python environment:

```
source preinstall.sh
pip install --target devsim_macos_arm64_2.8.1 devsim-2.8.1-cp37-abi3-macosx_12_0_universal2.whl
chmod u+x devsim_macos_arm64_2.8.1/devsim_data/testing/rundifftest.py
bash travis_tests.sh 2.8.1
```
