# Simple Image Generation with Stable Diffusion 1.5

This project serves as a beginner-friendly introduction to text-to-image generation using the Stable Diffusion 1.5 model. It's designed to be run in a Google Colab environment, allowing users to generate basic images from text prompts by executing cells sequentially.

This is a completed demo aimed at anyone looking to understand the fundamental steps involved in generating images from text.

## ✨ What it Does
*   Uses the **Stable Diffusion 1.5** model for image generation.
*   Generates images based on user-defined text prompts.
*   Designed for easy, cell-by-cell execution in **Google Colab**.
*   Optimized for use with a **T4 GPU** on Colab (though other GPUs might work).
*   Serves as an educational demo to introduce the basics of text-to-image pipelines.

## 🛠️ Prerequisites
*   A Google Account (for accessing Google Colab).
*   Basic familiarity with Jupyter Notebooks/Google Colab interface is helpful but not strictly necessary.

## 🚀 How to Use
1.  **Open in Colab:**
    *   Upload the `Simple Image Generation.ipynb` notebook to your Google Drive.
    *   Open it with Google Colaboratory.
    *   Alternatively, if you upload this project to GitHub, you can directly open the notebook in Colab using the "Open in Colab" badge (you can generate one or link directly).

2.  **Set Runtime Type:**
    *   In Colab, navigate to `Runtime` -> `Change runtime type`.
    *   Under `Hardware accelerator`, select `T4 GPU` (or another available GPU like V100, A100 if T4 is not listed).
    *   Click `Save`.

3.  **Run Cells Sequentially:**
    *   Execute each code cell in the notebook from top to bottom. You can do this by clicking the "Play" button to the left of each cell or by selecting a cell and pressing `Shift + Enter`.
    *   **Cell 1:** Installs the necessary `diffusers` library and its dependencies.
    *   **Cell 2 (and subsequent model loading cells):** Loads the Stable Diffusion 1.5 model pipeline from Hugging Face. This might take a few minutes as it downloads the model components. You'll see progress bars for the download.
    *   **Prompt Cell:** You'll find a cell similar to this:
        ```python
        prompt = "generate a madara uchiha pic"
        ```
        Modify the text within the quotes to describe the image you want to generate.
    *   **Generation Cell:** The final code cell will use the `pipeline` and your `prompt` to generate the image and display it. This step utilizes the GPU and may take a short while depending on the complexity and GPU availability.

## 📝 Example Prompt
The notebook comes with an initial prompt:
```python
prompt = "generate a madara uchiha pic"
