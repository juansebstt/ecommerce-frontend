# E-commerce Frontend

## Overview

The **E-commerce Frontend** is a web-based user interface for the e-commerce platform. Built using Angular, it allows users to browse products, manage their shopping cart, make payments, and access their account information seamlessly.

## Features

- **User Authentication**: Allows users to register, log in, and manage their accounts.
- **Product Browsing**: Displays a catalog of products with filtering and sorting options.
- **Shopping Cart Management**: Users can add, remove, and modify items in their shopping cart.
- **Checkout Process**: Guides users through payment processing and order confirmation.
- **Responsive Design**: Optimized for various devices, including desktops, tablets, and mobile phones.

## Technologies Used

- **Angular** (for building the frontend application)
- **NgRx** (for state management)
- **HttpClient** (for API requests)
- **Angular Material** or **Bootstrap** (for UI components)

## Prerequisites

Before running this service, ensure you have the following installed:

- **Node.js** and **npm** (Node Package Manager)
- Access to the backend services (e.g., API Gateway, Auth Service, Payment Service).

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/juansebstt/ecommerce-frontend.git
    ```

2. Navigate to the project directory:

    ```bash
    cd ecommerce-frontend
    ```

3. Install dependencies:

    ```bash
    npm install
    ```

4. Start the development server:

    ```bash
    ng serve
    ```


## Configuration

The frontend service may require configuration for connecting to backend services. Ensure to set the appropriate API URLs in your environment variables or configuration files.

### Sample Configuration

You may need to configure the following API endpoints in the `environment.ts` file:

```tsx
export const environment = {
  production: false,
  apiGatewayUrl: 'http://localhost:8080',
  authServiceUrl: 'http://localhost:8081',
  paymentServiceUrl: 'http://localhost:8082',
  productServiceUrl: 'http://localhost:8083',
  cartServiceUrl: 'http://localhost:8084',
  orderServiceUrl: 'http://localhost:8085',
  userServiceUrl: 'http://localhost:8086',
  notificationServiceUrl: 'http://localhost:8087',
  catalogServiceUrl: 'http://localhost:8088',
  commonServiceUrl: 'http://localhost:8089',
  contactServiceUrl: 'http://localhost:8090'
};

```

## Inter-Service Communication

The E-commerce Frontend connects with the following microservices:

- **[E-commerce API Gateway](https://github.com/juansebstt/ecommerce-api-gateway)**:
  - All requests from the frontend are routed through the API Gateway, which forwards them to the appropriate microservices.
- **[E-commerce Auth Service](https://github.com/juansebstt/ecommerce-auth-service)**:
  - Manages user authentication and authorization, providing JWT tokens for secure access.
- **[E-commerce Payment Service](https://github.com/juansebstt/ecommerce-payment-service):**
  - Handles payment processing when users make purchases.
- **[E-commerce Product Service](https://github.com/juansebstt/ecommerce-product-service)**:
  - Retrieves product details and availability for display in the frontend.
- **[E-commerce Cart Service](https://github.com/juansebstt/ecommerce-cart-service)**:
  - Manages users' shopping cart sessions and updates.
- **[E-commerce Order Service](https://github.com/juansebstt/ecommerce-order-service)**:
  - Handles order creation and management after checkout.
- **[E-commerce User Service](https://github.com/juansebstt/ecommerce-user-service)**:
  - Manages user profiles and account information.
- **[E-commerce Notification Service](https://github.com/juansebstt/ecommerce-notification-service)**:
  - Sends notifications and updates to users regarding their orders and account activities.
- **[E-commerce Catalog Service](https://github.com/juansebstt/ecommerce-catalog-service)**:
  - Provides detailed product information and availability.
- **[E-commerce Common Service](https://github.com/juansebstt/ecommerce-common-service)**:
  - Shares common utilities and components used across different services.
- **[E-commerce Contact Service](https://github.com/juansebstt/ecommerce-contact-service)**:
  - Manages customer support inquiries and communication.

## Usage

Once the frontend is running, you can access it via your web browser at `http://localhost:4200`. Users can perform actions like:

- Registering for an account
- Logging in and managing their profile
- Browsing products and adding them to the cart
- Checking out and making payments


This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 18.2.7.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.dev/tools/cli) page.

