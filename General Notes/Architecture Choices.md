Architecture: 

5-Tier Architecture
-Presentation Layer: Managing user interactions via web interface
-Application Layer: Coordinates application activities and processes business logic
-Business Logic Layer: Handles business logic (takes in specific input, puts out specific output)
-Data Access Layer: Handles database operations
-Database Layer: Actual database 

Chosen to ensure modularity between the primary functions of the web-app, increasing reusability and preventing bugs from interference between functionalities from occuring 

Modular Monolith Architecture 
Chosen for simplicity in building/testing/deploying 
    -Portfolio app is small enough that scaling is unnecessary for now
    -Should scaling be necessary, components should be written such that:
        -They can be easily extracted into their own microservice
        -They can recieve data from microservices without any change to themselves 
            -Code from microservices transfered using APIs that can adapt the data to a format that can be inputted directly into recieving component 
                -Connect components in Modular Monolith using thin dummy-APIs that can be swapped out for real APIs easily

Others:
    -Components should be reusable, consisting of one file each, takes in one set of input data and puts out one set of output data  
    -Connected with thin glue code

