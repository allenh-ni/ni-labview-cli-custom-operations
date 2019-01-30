# NI LabVIEW CLI - VIPM Operations Add-On
This add-on adds the following VIPM operations to the [NI LabVIEW Command Line Interface](http://www.ni.com/en-us/support/downloads/software-products/download.ni-labview-command-line-interface.html "NI LabVIEW CLI download"). This add-on supports LabVIEW 2014 or later.
* VIPM Install Package File
* VIPM Uninstall Package

## How to install
1. Install the [NI LabVIEW Command Line Interface](http://www.ni.com/en-us/support/downloads/software-products/download.ni-labview-command-line-interface.html "NI LabVIEW CLI download").
Note: LabVIEW 2018 or later automatically install the NI LabVIEW CLI.  However, you can also download and install it separately, and it supports LabVIEW 2014 or later.
2. Install the "NI LabVIEW Command Line Interface - VIPM Operations" add-on by downloading/installing the latest package (.nipkg) in the [Exports](https://github.com/allenh-ni/ni-labview-cli-custom-operations/tree/master/Exports) folder.
3. Install the [JKI VIPM API](http://sine.ni.com/nips/cds/view/p/lang/en/nid/210804) in all versions of LabVIEW you want to support. Note: This API requires the paid VIPM Pro license.


## How to use
Run the following commands from the command-line interface.

### VIPMInstallPackageFile
`LabVIEWCLI -OperationName VIPMInstallPackageFile -PackagePath <path of VIPM package file (.vip)> -LabVIEWVersion <labview version string>`

-PackagePath : Specifies the path to the VIPM package file (.vip) to install

-LabVIEWVersion : Specifies the version of LabVIEW to install the VIPM package to (e.g. "17.0", "17.0 (64-bit)", "18.0", "18.0 (64-bit)", ...)

### VIPMInstallPackageFile
`LabVIEWCLI -OperationName VIPMUninstallPackage -PackageName <package name> -LabVIEWVersion <labview version string>`

-PackageName: Specifies the name of the VIPM package to install (e.g. package_abc_api-2.5.0.0)

-LabVIEWVersion : Specifies the version of LabVIEW to uninstall the VIPM package from (e.g. "17.0", "17.0 (64-bit)", "18.0", "18.0 (64-bit)", ...)


## Reference
For more information on how to create/install custom NI LabVIEW CLI operations, refer to this [help topic](http://zone.ni.com/reference/en-XX/help/371361R-01/lvhowto/cli_creating_operations/ "Creating Custom NI LabVIEW CLI Operations").
