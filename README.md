# sync-async-api-tutorial

## About
The Jupyter Notebook api_comparison.ipynb demonstrates how to make both synchronous and asynchronous API requests using the IUCN API as an example.

In the tutorial, the following areas are covered:
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

### Prerequisites
This tools relies on API calls to IUCN. *The IUCN API is a RESTful API that provides access to data from the International Union for Conservation of Nature (IUCN). The API allows users to query for information about species, habitats, and other conservation-related data.* 

You will need setup an account with these organisations and request an API key. You can register here: https://apiv3.iucnredlist.org/.
Once you have the API key, copy it into a config.ini file in the root of the folder. Your config.ini file should look like this:
```
[API]
iucn = you_iucn_api
```

**Steps for running notebook on device**
1. Download zip from GitHub
2. Move the zipped folder to your documents folder on your device
3. Unzip the sync-async-api-tutorial folder
4. Open Anaconda prompt and change directory to the location of the sync-async-api-tutorial folder: `cd C:/path_to/sync-async-api-tutorial`
5. Setup the conda environment for the project by running the following line in the Prompt: `conda env create --name envname --file=environment.yaml`
6. Activate the conda environment: `conda activate api-env`
7. Go back to the sync-async-api-tutorial folder and open the api_comparison.ipynb file in Visual Studio Code
8. Click 'View', 'Command Palette' and type 'Python: Select Interpreter' into the search bar, choose the api-env environment
9. Run the api_comparison.ipynb notebook
