## MP 2 Data Processing REST API
The project uses FastAPI to create a REST API which allows users to upload, validate, process, and retrieve CSV datasets. MP2 continues work from MP1 whcih cleaned and validated the data. 

Some libraries that are used are pandas (data manipulation), Pydantic (request and response models), and in memory storage for the uploaded datasets. There is also different levels of logging for erros and warnings. 

The API endpoints are: 
- Checking if the API is running: the method is GET and the endpoint is /health
- Uploading and storing the CSV dataset: the method is POST and the endpoint is /uplaod
- Retrieves a stored dataset: the method is GET and the endpoint is /datasets/{dataset_id}
- Validating and cleaning a stored dataset based on user-provided settings: the method is POST and the endpoint is /datasets/{dataset_id}/process 


