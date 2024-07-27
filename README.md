# Product Service for E-commerce Application

This project is a Product Service for an e-commerce clothing application. The Product Service is designed to manage clothing products, encompassing various attributes such as brand, color, size, season, and more. By centralizing product management, it ensures consistency and accuracy across all product-related data on the e-commerce platform.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Service](#running-the-service)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Product Service is a RESTful API built using Spring Boot. It provides endpoints for creating, updating, retrieving, and deleting clothing products. This service integrates with other microservices to manage attributes like brand, color, size, and season, ensuring that all product data is accurate and up-to-date.

## Features

- **Create Products:** Allows the creation of new clothing products with attributes such as brand, color, size, and season.
- **Retrieve Products:** Enables fetching details of existing products, supporting features like product filtering and search.
- **Update Products:** Allows updating attributes of existing products.
- **Delete Products:** Provides the ability to delete products from the system.

## Prerequisites

- Java 17 or higher
- Maven 3.6.3 or higher
- Spring Boot 3 or higher

## Installation

1. Clone the repository:

    - ```sh
      git clone https://github.com/Agustin199811/product-service.git
      cd product-service
      ```

2. Build the project using Maven:

    - ```sh
      mvn clean install
      ```

## Configuration

The configuration for the Product Service is located in `src/main/resources/application.properties`. Below is an example configuration:

```properties
spring.datasource.url=jdbc:mysql://clot.cp88o8squjfi.us-east-1.rds.amazonaws.com:3306/clot
spring.datasource.username=root
spring.datasource.password=root1234

eureka.client.service-url.defaultZone=http://clot-ecommerce-ELB-1792240696.us-east-1.elb.amazonaws.com:8761/eureka/
eureka.client.register-with-eureka=true
eureka.client.fetch-registry=true
```

## Running the Service

To run the service registry, use the following command:

 ```sh
    mvn spring-boot:run
```

## Contributing

Contributions are welcome! If you would like to contribute to this project, please send us an email at
`toapantaagustin9c@gmail.com` with details about your proposed changes or improvements. We look forward to hearing from you!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
