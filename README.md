# 🌍 GeoJSON2XML 🛠️

Code to transform your GeoJSON files into XML format.

## 🚀 Quick Install

1. **Download and install Miniconda** 🐍  
   If you don’t already have Miniconda, grab it [here](https://docs.anaconda.com/miniconda/) and follow the installation instructions. It’s painless, we promise.

2. **Create and activate your environment** 🧪  
   Open your terminal or command prompt and type the following magical incantations:

   ```sh
   conda create -n GeoJSON2XML python=3.9.19
   
   conda activate GeoJSON2XML
   ```

3. **Install GeoJSON2XML** 📦  
   Install the package directly from the source of truth (a.k.a. GitHub):

   ```sh
   pip install -e git+https://github.com/Valentinamatos/GeoJSON2XML.git#egg=GeoJSON2XML
   ```

   > ⚠️ **Warning:**  
   > You might need to install Git from the following [🔗 link](https://git-scm.com/downloads/win) to be able to run the `pip install` git link command.

   > ⚠️ **Warning:**  
   > After installing the package, restart your IDE and activate the environment again using `conda activate GeoJSON2XML` to ensure all the dependencies are properly loaded.

## ⚙️ How to Use

1. **Prepare Your GeoJSON Files**:  
   Place all the GeoJSON files you want to convert into a single folder. This ensures consistent label ordering across all files.

2. **Run the Jupyter Notebook**:  
   Open the `GeoJSON2XML.ipynb` notebook in your Jupyter environment. Run the following cells:

   - Import the required module:
     ```python
     from base import *
     ```
   - Set the path to your folder containing GeoJSON files:
     ```python
     folder_path = r'path to GeoJSON files'
     ```
   - Run the conversion:
     ```python
     GeoJSON2XML(folder_path)
     ```

   This will process all GeoJSON files in the specified folder and generate corresponding XML files.

3. **Check the Output**:  
   The XML files will be saved in the same folder as the input GeoJSON files, with the `.xml` extension.

## ⚠️ Important Warnings

1. **Consistent Layer Order**:  
   To ensure that the generated XML files maintain the same order of layers, **all GeoJSON files that are to be converted must be placed in the same folder**. This guarantees consistent label ordering across all files.

Happy converting! 🎉

