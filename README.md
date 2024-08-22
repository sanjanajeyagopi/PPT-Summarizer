# PPT-Summarizer
### README.md

# PPT Content Analyzer

This project provides a comprehensive solution for analyzing the content of PowerPoint presentations by extracting images and text, generating captions for images, summarizing slide text, and compiling the results into a PDF report. The project leverages advanced models like BLIP for image captioning and BART for text summarization.

## Features

- **Image Extraction**: Extracts images from each slide in the PowerPoint presentation.
- **Image Captioning**: Uses BLIP (Salesforce/blip-image-captioning-large) to generate captions for the extracted images.
- **Text Extraction**: Extracts text from each slide.
- **Text Summarization**: Summarizes the extracted text using BART (facebook/bart-large-cnn).
- **PDF Report Generation**: Combines the captions and text summaries into a layman-friendly PDF report.

## Installation

To run this project in Google Colab, you need to install the following dependencies:

```bash
pip install transformers python-pptx Pillow fpdf torch
```

## Usage

1. **Upload the PowerPoint File**: Upload your `.pptx` file when prompted.

2. **Generate Report**: The notebook will extract images and text, perform captioning and summarization, and generate a downloadable PDF report with the combined information.

### Steps

- **Clone the Repository**:
  ```bash
  git clone https://github.com/yourusername/PPT-Content-Analyzer.git
  cd PPT-Content-Analyzer
  ```

- **Run the Notebook**:
  Open the provided notebook in Google Colab or Jupyter Notebook and follow the instructions to upload your PowerPoint file and generate the report.

## File Structure

- **`extract_images_from_ppt()`**: Function to extract images from the PowerPoint slides.
- **`generate_image_captions()`**: Function to generate captions for the extracted images using BLIP.
- **`extract_text_from_ppt()`**: Function to extract text from each slide.
- **`summarize_text()`**: Function to summarize the extracted text using BART.
- **`create_pdf_report()`**: Function to compile the captions and summaries into a PDF report.

## Dependencies

- **Python 3.7+**
- **Google Colab/Jupyter Notebook**
- **Libraries**:
  - `transformers`
  - `python-pptx`
  - `Pillow`
  - `fpdf`
  - `torch`

## Examples

Here's an example of how the captions and summaries might look in the generated PDF:

```
Slide 1:
Image Description: "A group of people working together in an office."
Slide Summary: "This slide discusses the importance of collaboration in modern workplaces..."

Slide 2:
Image Description: "A chart showing the growth in revenue over the past year."
Slide Summary: "This slide highlights the significant increase in revenue..."
```


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- This project utilizes models and tools from the Hugging Face Transformers library.
- Special thanks to the open-source community for providing the tools and resources that made this project possible.

---

This README provides a comprehensive guide to understanding, installing, and using the PPT Content Analyzer. It is structured to make it easy for anyone, from beginners to advanced users, to contribute to or use the project effectively.
