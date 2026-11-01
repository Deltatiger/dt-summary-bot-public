The objective of this feature is to ensure that some emails with complex images are all processed correctly. To achieve this, make the following changes.

1. In the Email service, do not replace the image tags.
2. In the processor, if image tag processing is required, then do the following things for each image.
3. For each image, download the image data from the server.
4. Using the Google Cloud API, send the image to the Gemini flash model and ask it to decode the image. Ensure that the image processing prompt comes from the derived class.
5. Replace the img tag with the new summary from the google cloud API.
6. Send the data to the LLM for complete summary, just like the other items.