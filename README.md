# Install Deep Learning Libraries for NVIDIA Jetson

This guide provides instructions on installing deep learning libraries on NVIDIA Jetson devices. 


## As an example, we will install **ONNX** on **JetPack 5.1.2** with **Python 3.8**.

## Prerequisites
- NVIDIA Jetson device with JetPack installed
- Internet connection
- Terminal access

## Step 1: Check Installed JetPack Version
To verify the installed JetPack version, run:

```bash
apt-cache show nvidia-jetpack
```

Ensure that the version displayed matches **JetPack 5.1.2**. (Example)

## Step 2: Check Python Version
Verify the installed Python version:

```bash
python3 --version
```

Ensure that the version displayed is **Python 3.8**. (Example)

## Step 3: Download the Deep Learning Library
1. Open a web browser and go to the Jetson Zoo website:
   - [Jetson Zoo](https://elinux.org/Jetson_Zoo)
2. Scroll to the **Deep Learning Libraries** section.
3. Locate **ONNX** and ensure compatibility with **JetPack 5.1.2** and **Python 3.8**.
4. Click the download link to get the appropriate **.whl** file.

## Step 4: Install the Library
Once the download is complete:

1. Open a terminal and navigate to the directory where the file was downloaded:
   
   ```bash
   cd /path/to/downloaded/file
   ```

2. Install the ONNX library using `pip`:
   
   ```bash
   python3 -m pip install onnx-<version>.whl
   ```

Replace `onnx-<version>.whl` with the actual filename of the downloaded ONNX package.

## Step 5: Verify Installation
To confirm that the library was installed successfully, run:

```bash
python3 -c "import onnx; print(onnx.__version__)"
```

This should display the installed ONNX version.

## Customizing for Other Libraries
To install a different deep learning library, follow the same steps but select the desired library from the Jetson Zoo website and install its corresponding `.whl` file.

## Conclusion
Following these steps, you can install and verify deep learning libraries on your NVIDIA Jetson device. This guide uses ONNX as an example, but the same process applies to other libraries available in Jetson Zoo.

