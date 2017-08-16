# Material for Code4Lib Paper on OXPath

This repository contains accompanying material to our article submitted to the Code4Lib Journal.

## Getting Started

To get a copy of the materials, use either `git clone`, or download the repository's content as a compressed file (.zip) and extract it anywhere on your local file system.

### Prerequisites

Currently, OXPath is only supported on 64bit Linux-based operating systems. Java has to be installed on this system (version 8 or above). Optionally, the xvfb package has to be installed if you want to use the option to run Firefox in the X virtual framebuffer for the evaluation of OXPath expressions.

### Installation of XVFB (e.g. on Ubuntu 16.04)

```sh
$ sudo apt install xvfb
```

### Get OXPath

OXPath can be obtained from: [www.oxpath.org/download](http://www.oxpath.org/download)
Pick the latest version of the CLI jar and save it to a convenient location.

## Running the example

### With OXPath 2.0

To run the example, fire up a command line and input the following command, where

-   `-query bicc_WP.oxp`: reads the OXPath expression in the file `bicc_WP.oxp`
-   `-logfile VerboseLog4j.properties`: uses the provided custom logging configuration file for more verbose logging (recommended for OXPath beginners)
-   `-browser firefox_xvfb`: runs the OXPath evaluation with a virtual frame buffer
-   `-output bicc_WP.xml`: re-directs the XML output to the file `bicc_WP.xml`
-   `-xml`: sets the output format to XML

```sh
$ java -jar oxpath-2.0-cli.jar -query bicc_WP.oxp -logfile VerboseLog4j.properties -browser firefox_xvfb -output bicc_WP.xml -xml
```
### With OXPath 2.0.2

(will be released soon, more info to follow)
<!--- Note to self: adjust when new version is officially released --->
<!--
To run the example, fire up a command line and input the following command, where

-   `-q bicc_WP.oxp`: reads the OXPath expression in the file `bicc_WP.oxp`
-   `-log VerboseLog4j.properties`: uses the provided custom logging configuration file for more verbose logging (recommended for OXPath beginners)
-   `-xvfb`: (optional) runs the OXPath evaluation with a virtual frame buffer
-   `-o bicc_WP.xml`: re-directs the XML output to the file `bicc_WP.xml`

```sh
$ java -jar oxpath-2.0-cli.jar -q bicc_WP.oxp -log VerboseLog4j.properties -xvfb -o bicc_WP.xml
```
-->

## Author

*   **Mandy Neumann** - *Lead author of the article*

## License

This project is licensed under the Apache 2.0 License - see the [LICENSE.md](LICENSE.md) file for details.

<!--The OXPath executable contained in this repository is licensed under Apache 2.0 License.-->

## Acknowledgments

*   **Jan Steinberg** - *Contributor of the OXPath expression script and second author*
*   **Philipp Schaer** - *Third author and proof-reader*
