# Azure AI Vision - Image Analysis API

## The Azure AI Vision 
Image Analysis API leverages Azure's Cognitive Services to perform detailed analyses on images. It extracts information, detects objects, and provides insights into visual content.

### Features

    Image Analysis: This feature analyzes images to extract important information, identify objects, and provide insights into the content.

### API Endpoints
1. Image Analysis

This endpoint allows you to analyze an image and obtain detailed information about its content.

    Endpoint: http://167.71.80.195:3000/Process_Image
    Method: GET
    Headers:
        Key: Content-Type, Value: application/json
    Query Parameters:
        Name: imageUrl
        Type: string
        Required: Yes
        Description: URL of the image to be analyzed
        Example: http://167.71.80.195:3000/Process_Image?imageUrl=https://img.freepik.com/free-photo/young-bearded-man-with-striped-shirt_273609-5677.jpg

### Example Request

Here are the links to the example images demonstrating how to use the endpoint:

*Endpoint Screenshots*

<img src="https://github.com/Shrey85/sysint-images/blob/main/1.png" alt="Image description" width="600" height="400"/>

<img src="https://github.com/Shrey85/sysint-images/blob/main/2.png" alt="Image description" width="600" height="400"/>

<img src="https://github.com/Shrey85/sysint-images/blob/main/3.png" alt="Image description" width="600" height="400"/>

*POSTMAN Screenshot*

<img src="https://github.com/Shrey85/sysint-images/blob/main/4.png" alt="Image description" width="600" height="400"/>

*Responses*

| Status Code | Response                     | Description                                                        |
|-------------|------------------------------|--------------------------------------------------------------------|
| 200         | Successful Response          | The API will return detailed information about the analyzed image. |
| 400         | Invalid Image URL Provided   | Occurs when the provided image URL is not valid or missing.        |
| 500         | Internal Server Error        | General server error when the API fails to process the request.    |

### Getting Started

To use the Image Analysis API, follow these steps:
   
    Obtain an API Key: Ensure you have an API key from Azure configured in your environment.

### Usage

    Make a Request: Use the Process_Image endpoint to submit an image for analysis.
    Receive Results: Obtain detailed insights and information about the content of the submitted image.

## Limitations

1. **Environment Variables**:
    - The application relies on environment variables (`AZURE_API_ENDPOINT` and `AZURE_API_KEY`) for configuration. Ensure these are set correctly in the `.env` file.

2. **Image URL**:
    - The API requires a valid image URL to be provided as a query parameter. If an invalid URL is provided, the API will return a `400` status code with an appropriate error message.

3. **Supported Image Formats**:
    - The API only supports certain image formats (JPEG, PNG, GIF, BMP, TIFF). Ensure the image URL points to an image in one of these formats.

4. **Image Size**:
    - There is a limitation on the image size that can be processed. If the image is too large, the API will return an error indicating that the image size is too large.


### License

This project is licensed under the Shresta Varma - see the LICENSE.md file for details.
Additional Information

Ensure that the URLs provided for the images are correct and that the images are accessible to your audience. If the images are meant to be viewed by a restricted audience, consider adjusting the permissions accordingly.
