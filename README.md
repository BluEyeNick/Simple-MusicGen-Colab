# MusicGen Colab Notebook

This Jupyter notebook provides an easy interface for generating musical audio using Facebook's MusicGen AI model. It allows anyone to quickly generate original music clips by simply providing text prompts.

## Features

- User-friendly forms to configure generation parameters like prompt text, duration, etc.
- Automatically handles loading the MusicGen model and dependencies.
- Generates multiple audio clips per prompt to explore variation.
- Cleans and formats prompt text to use as audio file names. 
- Saves results organized into folders on Google Drive for easy access.
- Includes logic to only load libraries once across notebook re-runs.
- Detailed comments explaining each step of the process.

## Usage

After opening the notebook in Colab:

1. Update any settings in the forms at the top like duration, number of outputs, and prompt texts.
2. Run all cells using the "Runtime > Run All" menu option.
3. Generated audio files and text prompts will be saved to your Google Drive under /MusicGen/{prompt}.
4. Listen to the generated tracks right within Colab!

## Implementation

The notebook utilizes Facebook's pre-trained MusicGen models along with the audiocraft Python package. It generates audio waveform data directly from the model using the provided text prompts. This data is then written to WAV files using SciPy.

Key steps:

- Install audiocraft package 
- Load pre-trained MusicGen model
- Take user inputs from forms 
- Format prompt texts
- Generate audio samples
- Write audio data to WAV files
- Organize and name output files

By packaging this logic into an easy-to-use Colab notebook, this tool makes AI music generation accessible to everyone!

## Credits

MusicGen model and audiocraft library developed by Facebook AI Research. Notebook created by BluEyeNick.
