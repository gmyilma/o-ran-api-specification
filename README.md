
# Unified Network Slice Lifecycle Management API

This repository contains the Swagger specification for the Unified Network Slice Lifecycle Management API. The API defines the endpoints and their functionalities for managing network slices in a unified manner.

## Getting Started

To use the Unified Network Slice Lifecycle Management API, follow these steps:

1. Clone the repository to your local machine:



2. Review the Swagger specification file:

- Open `oran-api-spec-swagger.yaml` to access the detailed API documentation. The specification provides information about each endpoint, including the supported methods, input parameters, and expected responses.

3. Choose a method to interact with the API:

- Use a Swagger UI tool like [Swagger UI](https://swagger.io/tools/swagger-ui/) or [ReDoc](https://redoc.ly/) to visualize and test the API endpoints directly from the Swagger specification file.

- Integrate the API into your application or tool by generating client code or using libraries compatible with Swagger specifications. You can use tools like [Swagger Codegen](https://swagger.io/tools/swagger-codegen/) to generate client code in various programming languages.

  - example end point https://app.swaggerhub.com/apis/gmyilma/unified-network_slice_lifecycle_management_api/1.0.0

## API Endpoints

The following API endpoints are available:

### NSSMF_NonRTRIC

#### Create a new NSSMF-Non-RT RIC entry

- **Endpoint:** `POST /NSSMF_NonRTRIC`
- **Summary:** Create a new NSSMF-Non-RT RIC entry.
- **Description:** Creates a new entry for the NSSMF-Non-RT RIC interface.
- **Parameters:**
- `nssmfNonRtricRequest` (body): Request parameters for NSSMF-Non-RT RIC interface (see `NSSMFNonRTRICRequest` definition).
- **Response:**
- `200`: Successful response.

#### Get an NSSMF-Non-RT RIC entry by ID

- **Endpoint:** `GET /NSSMF_NonRTRIC/{id}`
- **Summary:** Get an NSSMF-Non-RT RIC entry by ID.
- **Description:** Retrieves an existing NSSMF-Non-RT RIC entry by ID.
- **Parameters:**
- `id` (path): The ID of the NSSMF-Non-RT RIC entry.
- **Response:**
- `200`: Successful response.

#### Update an NSSMF-Non-RT RIC entry by ID

- **Endpoint:** `PUT /NSSMF_NonRTRIC/{id}`
- **Summary:** Update an NSSMF-Non-RT RIC entry by ID.
- **Description:** Updates an existing NSSMF-Non-RT RIC entry by ID.
- **Parameters:**
- `id` (path): The ID of the NSSMF-Non-RT RIC entry.
- `nssmfNonRtricRequest` (body): Updated request parameters for NSSMF-Non-RT RIC interface (see `NSSMFNonRTRICRequest` definition).
- **Response:**
- `200`: Successful response.

#### Delete an NSSMF-Non-RT RIC entry by ID

- **Endpoint:** `DELETE /NSSMF_NonRTRIC/{id}`
- **Summary:** Delete an NSSMF-Non-RT RIC entry by ID.
- **Description:** Deletes an existing NSSMF-Non-RT RIC entry by ID.
- **Parameters:**
- `id` (path): The ID of the NSSMF-Non-RT RIC entry.
- **Response:**
- `200`: Successful response.

### NFVO_NonRTRIC

#### Create a new NFVO-Non-RT RIC entry

- **Endpoint:** `POST /NFVO_NonRTRIC`
- **Summary:** Create a new NFVO-Non-RT RIC entry.
- **Description:** Creates a new entry for the NFVO-Non-RT RIC interface.
- **Parameters:**
- `nfvoNonRtricRequest` (body): Request parameters for NFVO-Non-RT RIC interface (see `NFVONonRTRICRequest` definition).
- **Response:**
- `200`: Successful response.

#### Get an NFVO-Non-RT RIC entry by ID

- **Endpoint:** `GET /NFVO_NonRTRIC/{id}`
- **Summary:** Get an NFVO-Non-RT RIC entry by ID.
- **Description:** Retrieves an existing NFVO-Non-RT RIC entry by ID.
- **Parameters:**
- `id` (path): The ID of the NFVO-Non-RT RIC entry.
- **Response:**
- `200`: Successful response.

#### Update an NFVO-Non-RT RIC entry by ID

- **Endpoint:** `PUT /NFVO_NonRTRIC/{id}`
- **Summary:** Update an NFVO-Non-RT RIC entry by ID.
- **Description:** Updates an existing NFVO-Non-RT RIC entry by ID.
- **Parameters:**
- `id` (path): The ID of the NFVO-Non-RT RIC entry.
- `nfvoNonRtricRequest` (body): Updated request parameters for NFVO-Non-RT RIC interface (see `NFVONonRTRICRequest` definition).
- **Response:**
- `200`: Successful response.

#### Delete an NFVO-Non-RT RIC entry by ID

- **Endpoint:** `DELETE /NFVO_NonRTRIC/{id}`
- **Summary:** Delete an NFVO-Non-RT RIC entry by ID.
- **Description:** Deletes an existing NFVO-Non-RT RIC entry by ID.
- **Parameters:**
- `id` (path): The ID of the NFVO-Non-RT RIC entry.
- **Response:**
- `200`: Successful response.

### NSSMF_Termination

#### Message exchange between NSSMF and Non-RT RIC

- **Endpoint:** `POST /NSSMF_Termination`
- **Summary:** Message exchange between NSSMF and Non-RT RIC.
- **Description:** Facilitates message exchange between NSSMF and Non-RT RIC via the NSSMF_NonRTRIC interface.
- **Parameters:**
- `nssmfTerminationRequest` (body): Request parameters for NSSMF Termination (see `NSSMFTerminationRequest` definition).
- **Response:**
- `200`: Successful response.

### NFVO_Termination

#### Message exchange between NFVO and Non-RT RIC

- **Endpoint:** `POST /NFVO_Termination`
- **Summary:** Message exchange between NFVO and Non-RT RIC.
- **Description:** Facilitates message exchange between NFVO and Non-RT RIC via the NFVO_NonRTRIC interface.
- **Parameters:**
- `nfvoTerminationRequest` (body): Request parameters for NFVO Termination (see `NFVOTerminationRequest` definition).
- **Response:**
- `200`: Successful response.

## Contributing

Contributions are welcome! If you have any suggestions, improvements, or bug fixes, please submit a pull request. Before submitting a pull request, make sure to run the tests and ensure they pass.

## License

This project is licensed under the [MIT License](LICENSE).
