# CovidGuardPriv
This is the artifact accompanying the submission "An Empirical Assessment of Global COVID-19 Contact Tracing Applications".

The original results are produced on a workstation with xxx CPU (x cores, x GHz), x GB RAM, and the operating system is xxx. To reproduce the results, a machine with similar CPUs(~2.10GHz), x GB or larger RAM is required. Running the artifact on a different machine could possibly diverge the execution and lead to different results.   

## Setup
This project requires python3 and Java environment. 
So please ensure you have installed **python3 (>=3.6)**, **Java (>=8)** and **Android SDK**.

Please run following commands in your PowerShell or CMD prompt in Windows, or shell in *nix/macOS
```bash
 $ python3 -m venv
 $ source venv
 $ python3 -m pip install -r requirement.txt
```

If you want to verify apk files through VirusTotal, please input your api_key of VirusTotal in assets/virus_total.yaml

## Usage
#### 1. Clone COVIDGuardian repo.
```bash
  $ git clone https://github.com/covid-guardian/covid-guardian 
```
#### 2. Run main.py

```
usage: python main.py [-h] -s ANDROID_SDK_PATH [-n PARALLEL_NUMBER] APK_OR_DIRECTORY_PATH

```
Mandatory arguments:
* `-s ANDROID_SDK_PATH` is used to set the path to the Android SDK
* `APK_PATH` is used to set the path to the APK file or a directory containing APK files

Optional arguments:
* `-h, --help` is used to show the help message and exit
* `-n PARALLEL_NUMBER` is used to set the number of parallel works, default is the number of CPU cores
## Example

