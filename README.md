# COS 791 - Image Processing
## Assignment 2 - Multilevel Thresholding

### Introduction
In this assignment we were tasked to implement two algorithms that would help optimize the multilevel threshold methods (**Otsu** and **Kapur**) by finding an optimal combination of threshold values. The two algorithms that we had to implement are:
- Simulated Annealing (SA)
- Variable Neighbourhood Search (VNS)
We evaluated the algorithms using the Otsu and Kapur objective functions as well as the quality metrics **structural similarity (SSIM)** and **peak-signal noise ratio**. Finally, we evaluated these algorithms across a range of threshold levels: 2, 3, 4, and 5.

Below we show an example of the SA algorithm's output for threshold levels 2, 3, 4, and 5, respectively. All of the output images for the respective algorithms and thresholding methods and levels can be found inside the `output` directory.

<div align='center'>
  <label>Level 2</label>
  <img src='https://github.com/JsteReubsSoftware/COS791-Assignment2/blob/main/output/SA_Otsu_output_imgs_T42.jpg/SA_Otsu_level_2_output_T42.jpg.png' altText='example output' />
  <label>Level 3</label>
  <img src='https://github.com/JsteReubsSoftware/COS791-Assignment2/blob/main/output/SA_Otsu_output_imgs_T42.jpg/SA_Otsu_level_3_output_T42.jpg.png' altText='example output' />
  <label>Level 4</label>
  <img src='https://github.com/JsteReubsSoftware/COS791-Assignment2/blob/main/output/SA_Otsu_output_imgs_T42.jpg/SA_Otsu_level_4_output_T42.jpg.png' altText='example output' />
  <label>Level 5</label>
  <img src='https://github.com/JsteReubsSoftware/COS791-Assignment2/blob/main/output/SA_Otsu_output_imgs_T42.jpg/SA_Otsu_level_5_output_T42.jpg.png' altText='example output' />
</div>

### How to run the program:
1. Clone the repository to your local environment by running the following command in your terminal: <br>
`git clone https://github.com/JsteReubsSoftware/COS791-Assignment2.git`
2. Copy the entire folder to your Google Drive *(the Notebook file was developed on Google Colab and thus uses specific file paths)*
3. Open the **Jupyer Notebook** file `u21457060-cos791-a2.ipynb`
4. Search for all the file paths starting with `/content/drive/MyDrive/University/Honours/COS791/Assignments` and replace them with the path `/content/drive/<your-directory>` where `<your-directory>` refers to the path where you uploaded the repository folder on your Google Drive.
5. Once the file paths are correctly setup you can simply run the notebook from top to bottom. The **Main Program** section contains the code for running both the SA and VNS algorithms.

**Note: The implementation for the functions `calc_variance` and `calc_entropy` was adapted from the `_get_variance` and `_get_enropy` functions found in the open source library [pythreshold](https://github.com/manuelaguadomtz/pythreshold/tree/master).**

**We adapted these functions to fit to the need of our assignment and due to the functions being **private** we were unable to import them directly.**
