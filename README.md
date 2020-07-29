## A quickstart guide on interacting with your Canvas courses via the unofficial Python API

Canvas has a well developed API, and there is an unofficial [Python wrapper for this API](https://github.com/ucfopen/canvasapi), developed by the University of Central Florida. The main Canvas API is available at https://canvas.instructure.com/doc/api/index.html.

In this repo/notebook we will see an outline of how the Python wrapper can be used to interact with the Canvas courses. Of course, depending on your level of access, you can use the API get/edit any Canvas data of interest. [The details are in the documentation](https://canvasapi.readthedocs.io/en/stable/).

### Prerequisites: 

Familiarity with Python, virtual environments, handling sensitive credentials, interacting with APIs. Remember, it's all too easy to delete an entire course using one command!

**If you are sharing your scripts online/with others, be sure to omit the credential token.**

### Steps:

1. Go to Account -> Settings -> New Access Token, and create a new token. Copy the token and paste it on a text file as plain text. For this example, let's assume that the token is "abcd1234".

2. Install CanvasAPI Python wrapper via pip ("pip install canvasapi"). It's *very strongly* recommended that you install it inside a virtual environment to leave your system Python installation untouched.

3. It might be easier to organize if you create one dedicated folder to store the credential file (containing the token) and the Python scripts, and use sub-folders ("data_upload" and "data_download" in this example) to get stuff in and out of your Canvas courses. Alternatively, you can change the paths of upload/download destinations for the specific courses as you use them.

Note: For this example, a cred.json file is included to demonstrate where you may keep your token. Remember to exclude this file/purge information from the notebook if you are sharing your scripts.
