# Distributed File System

#### Team Members:

- Amey Choudhary 
- Jainit Bafna 
- Yash Bhaskar

We have designed and developed a distributed file system, which allows users to perform file operations and file management on files stored over distributed storage servers. The system integrates multiple storage servers and simplifies the user experience, akin to being on a single server. It has been implemented in C. The following is the [Project Description](https://karthikv1392.github.io/cs3301_osn/project/).

#### 
High-Level Modules
Client Module - handles client interactions, such as reading, writing, and obtaining information about files.
Naming Server Module - the central server that manages directories and file locations.
Storage Server Module - responsible for the actual data storage and file operations.
Communication Module - handles all network communication using TCP sockets.
Concurrency Module - handles concurrent client access and file operations.
Error Handling Module - defines and processes error codes.
Search Optimization Module - optimizes search operations within the Naming Server.
Redundancy Module - handles redundancy and replication of data.
Logging Module - for logging and message display.


Client Module Functions
connectToNamingServer()
sendReadRequest()
sendWriteRequest()
sendInfoRequest()
sendCreateRequest()
sendDeleteRequest()
sendCopyRequest()


Naming Server Module Functions
initializeNamingServer()
registerStorageServer()
handleClientRequest()
instructStorageServer()
searchForFile()
cacheSearchResult()
detectStorageServerFailure()
handleReplication()


Storage Server Module Functions
initializeStorageServer()
reportToNamingServer()
handleRequestFromNamingServer()
readFile()
writeFile()
getFileInfo()
createFileOrDirectory()
deleteFileOrDirectory()
copyFileOrDirectory()


Communication Module Functions (Using TCP Sockets)
openSocket()
acceptConnection()
readFromSocket()
writeToSocket()
closeSocket()



Concurrency Module Functions
processMultipleRequests()
lockFileForWrite()
unlockFile()



Error Handling Module Functions
defineErrorCodes()
handleError()



Search Optimization Module Functions
performEfficientSearch()
implementLRUCache()



Redundancy Module Functions
replicateData()
restoreFromReplica()
asynchronousReplication()



Logging Module Functions
logRequest()
logAck()
logError()
displayMessage()
