# Weather-Alert-Processor-Subscriber-
PATTERN
Subscribe Model : 

The Weather Alert Processor acts as a subscriber to this message queue.

The Subscribe Model in the context of the Weather Alert Processor is a design pattern that it  enables the system to consume and process weather alert messages in an asynchronous.

SOLUTION DESIGN
The system is designed to consume weather alert events, store them in a database, and expose APIs to access the alert data.

Queueing Mechanism:  Alerts are sent to a message queue and When a new alert is published to the queue, the Weather Alert Processor subscribes to the message queue, consumes the weather alert, and processes the data.

Processing the Message:  Upon receiving the alert, the system processes the message, validating its content and extracting the relevant information such as city name, Alert type, Alert message, Temperature , Timestamp. Based on the temperature the alert message will generate.  

Database: This processed information is then stored in the local database for tracking.

Expose APIs: After storing the alerts, the users to query and access the weather alert data.

Error Handling : Global error handler catches errors and raises human-readable messages.

Unit Testing : Ensure that the flow works as expected.  The alert should be processed and logged successfully.

 
