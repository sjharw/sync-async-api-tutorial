# sync-async-api-tutorial

## About
This brief tutorial takes you through sync and async methods of making API requests, using the IUCN API as an example. In the tutorial, the following areas are covered:
- Making API requests with the `requests`, `futures`, `asyncio` and `aiohttp` libraries
- Timing API requests
- Plotting the results of API requests
- Testing API requests

## Background
In Python, synchronous and asynchronous API requests refer to different ways of sending and receiving data from an external API or web service.

Synchronous API requests are blocking, meaning that when a request is made, the program waits for the response to come back before continuing with any other tasks. This can be useful in situations where the response is required immediately and no other tasks need to be performed until the response is received.

On the other hand, asynchronous API requests are non-blocking, meaning that when a request is made, the program continues to execute other tasks while waiting for the response to come back. This can be useful in situations where multiple requests need to be made at the same time or when the response time is unpredictable, allowing the program to continue working on other tasks while waiting for the response.

The importance of synchronous and asynchronous API requests depends on the specific use case. For example, synchronous requests may be preferred when working with small, simple APIs that require immediate responses, while asynchronous requests may be necessary when working with large, complex APIs that require many requests to be made at the same time.

## Tech stack
- Anaconda3 (Conda) 22.11.1
- Python 3.10.0
- Visual Studio Code 1.71.2

## Setup
1. Download zip from GitHub
2. Move the zipped folder to your documents folder on your device
3. Unzip the sync-async-api-tutorial folder
4. Open Anaconda prompt and change directory to the location of the sync-async-api-tutorial folder: `cd C:/path_to/sync-async-api-tutorial`
5. Dowload the required dependencies for the project by running the following code in the Prompt: `conda env create --name envname --file=environments.yaml`
6. Go back to the sync-async-api-tutorial folder and open the api_comparison.ipynb file in Visual Studio Code
7. Run the code