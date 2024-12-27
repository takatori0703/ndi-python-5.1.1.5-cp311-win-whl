# ndi-python installaton for Python 3.11.1

## About

* This repository is intended to provide ndi-python built for Python 3.11.1 running on Windows.
* Originals
  * Repository: https://github.com/buresu/ndi-python.git
  * PyPI: https://pypi.org/project/ndi-python/

## Installaton Approach

### [Plan A] From a pre-built wheel file

* install with pip
  * `pip install <whl>`
* Build info
  * Build Environment
    * Windows 10
    * NDI SDK v6
    * Python 3.11.1
  * Sources
    * Original repository(No longer maintained?) :ndi-python 5.1.1.5
      * `git clone https://github.com/buresu/ndi-python.git --recursive`
    * :+1: Fork with applied pull requests
      * `git clone https://github.com/Ahua9527/ndi-python.git --recursive`
  * Build logs (excerpt)
    ```sh
      -- Building for: Visual Studio 17 2022
      -- Selecting Windows SDK version 10.0.22621.0 to target Windows 10.0.19045.
      -- The C compiler identification is MSVC 19.41.34123.0
      -- The CXX compiler identification is MSVC 19.41.34123.0
      -- pybind11 v2.9.2
      -- Performing Test HAS_MSVC_GL_LTCG
      -- Performing Test HAS_MSVC_GL_LTCG - Success
      -- Found NDI: C:/Program Files/NDI/NDI 6 SDK
      MSBuild のバージョン 17.11.9+a69bbaaf5 (.NET Framework)
    ```

### [Plan B] Build the repository by your self

* Install NDI SDK
  * https://downloads.ndi.tv/SDK/NDI_SDK/NDI%206%20SDK.exe
  * Or https://ndi.video/for-developers/ndi-sdk/download/
* Clone
  * Original repository(No longer maintained?) :ndi-python 5.1.1.5
    * `git clone https://github.com/buresu/ndi-python.git --recursive`
  * :+1: Fork with applied pull requests
    * `git clone https://github.com/Ahua9527/ndi-python.git --recursive`
  * `cd ndi-python`
* Build wheel package
  * `python setup.py bdist_wheel`

## Lisence

* ndi-python is MIT License
* NDI follows NDI's license

## Software Provision Disclaimer

> This software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.