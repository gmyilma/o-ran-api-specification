# API Specification

This API specification document provides details about the available endpoints and their corresponding interfaces. The API follows the Swagger version 2.0 specification.

## Endpoints

### SMO Framework-Cellular Site Interface

- **Endpoint**: `/o1`
- **Method**: GET
- **Summary**: SMO Framework-Cellular Site Interface
- **Description**:
  This proposed logical interface aims to connect the SMO Framework and cellular network sites in order to support FCAPS capabilities for the underlying cellular network sites.
  The scope of this interface is similar to the O1 interfaces that connect the SMO Framework to the O-RAN NFs.
  It is expected that this interface will align, to the extent possible, with the 3GPP specifications for element management in the RAN architecture.

### O-RU-Cellular Site Interface

- **Endpoint**: `/cellular-site/notification`
- **Method**: POST
- **Summary**: O-RU-Cellular Site Interface
- **Description**:
  The CellularSite Notification interface enables the logical functionalities of the O-RU, which are deployed on cellular network sites, to subscribe to events and/or status updates from the underlying cellular network sites.
  The cellular network sites will include event producers to allow radio resource workloads to receive events and/or status updates that are only known to the underlying cellular infrastructure.
  This interface is particularly important. [Girma's opinion on O-RU Pool...]

### NC-OBH Interface

- **Endpoint**: `/o2/nc-obh`
- **Method**: POST
- **Summary**: NC-OBH Interface
- **Description**:
  This interface logically connects the NC and OBH. It is utilized by the WIM and NC to manage the OBH transport links and orchestrate their respective networking resources.
  Further discussion of this interface is beyond the scope of this article.

### NC-OMH Interface

- **Endpoint**: `/o2/nc-omh`
- **Method**: POST
- **Summary**: NC-OMH Interface
- **Description**:
  This logical interface connects the NC and OMH. The WIM and NC utilize this interface to manage the OMH transport links and orchestrate their corresponding networking resources.
  The scope of this article precludes any further discussion of this interface.

### NC-OFH Interface

- **Endpoint**: `/o2/nc-ofh`
- **Method**: POST
- **Summary**: NC-OFH Interface
- **Description**:
  This interface connects the NC and OFH logically. The WIM and NC employ this interface to manage the OFH transport links and orchestrate their corresponding networking resources.
  A detailed analysis of this interface goes beyond the scope of this study.

### O-RAN NSSMF Termination

- **Endpoint**: `/o-ran-nssmf-termination`
- **Method**: POST
- **Summary**: O-RAN NSSMF Termination
- **Description**:
  The O-RAN NSSMF Termination enables the O-RAN NSSMF to send and receive messages to and from the Non-RT RIC Framework via the NSSMF_NonRTRIC interface.
  These messages include: (a) handshaking messages between the Non-RT RIC and 3GPP-NSMS; (b) ; (c) ; (d) ; and (e).

### NFVO Termination

- **Endpoint**: `/nfvo-termination`
- **Method**: POST
- **Summary**: NFVO Termination
- **Description**:
  The NFVO Termination facilitates the exchanges of messages between the NFVO
