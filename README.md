Azure AI Vision - Image Analysis API

The Azure AI Vision - Image Analysis API leverages Azure's Cognitive Services to perform detailed analyses on images. It extracts information, detects objects, and provides insights into visual content.
Features

    Image Analysis: This feature analyzes images to extract important information, identify objects, and provide insights into the content.

API Endpoints
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
        Example: http://167.71.80.195:3000/Process_Image?imageUrl=https://images.unsplash.com/photo-1714761867751-5842207f2f49?q=80&w=2564&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D

Example Request

Here are the links to the example images demonstrating how to use the endpoint:
Endpoint Screenshots

    Endpoint Screenshot 1: https://processimagesi.s3.amazonaws.com/1.png
    Endpoint Screenshot 2: https://processimagesi.s3.amazonaws.com/2.png
    Endpoint Screenshot 3: https://processimagesi.s3.amazonaws.com/3.png

POSTMAN Screenshot

    POSTMAN Screenshot: https://processimagesi.s3.amazonaws.com/4.png

Responses

    200 Successful Response: The API will return detailed information about the analyzed image.
    400 Invalid Image URL Provided: Occurs when the provided image URL is not valid or missing.
    500 Internal Server Error: General server error when the API fails to process the request.

Getting Started

To use the Image Analysis API, follow these steps:

    Obtain an API Key: Ensure you have an API key from Azure configured in your environment.
    Include the API Key in Request Headers: Use the key for authentication in the headers of your API requests.

Usage

    Make a Request: Use the Process_Image endpoint to submit an image for analysis.
    Receive Results: Obtain detailed insights and information about the content of the submitted image.

License

This project is licensed under the Shresta Varma - see the LICENSE.md file for details.
Additional Information

Ensure that the URLs provided for the images are correct and that the images are accessible to your audience. If the images are meant to be viewed by a restricted audience, consider adjusting the permissions accordingly.