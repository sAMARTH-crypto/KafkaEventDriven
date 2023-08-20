# Event-Driven Microservices with Spring Boot and Kafka

![Project Logo](link_to_logo_image)

Welcome to the **Event-Driven Microservices Project**, where we dive into the world of microservices architecture, leveraging the power of Spring Boot and Kafka. In this project, we demonstrate how to build a seamless order processing system using event-driven communication between different microservices.

## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Environment](#environment)
- [Project Structure](#project-structure)
- [Modules](#modules)
- [Base Domain](#base-domain)
- [Order Service](#order-service)
- [Stock Service](#stock-service)
- [Email Service](#email-service)
- [Setup and Configuration](#setup-and-configuration)
- [Getting Started](#getting-started)
- [Conclusion](#conclusion)

## Introduction

Microservices architecture is a game-changer in modern software development, enabling agility, scalability, and modularity. In this project, we take a deep dive into event-driven microservices, highlighting the power of Spring Boot and Kafka in building a responsive and efficient order processing system.

## Project Overview

Our project is divided into a parent module, "Kafka Microservices," and four child modules: "Base Domain," "Email Service," "Order Service," and "Stock Service." Each module plays a crucial role in our event-driven ecosystem, showcasing seamless communication and functionality.

## Environment

- Spring Boot
- Apache Kafka

## Project Structure

The modular structure of the project promotes clean separation of concerns, making maintenance and scalability a breeze.

## Modules

### Base Domain

The "Base Domain" module acts as the backbone of our communication between the producer and consumer. It contains two classes, OrderDetails and OrderEvent, enabling smooth data transfer.

### Order Service

The "Order Service" module encapsulates the process of order creation. It consists of submodules like "Kafka Topic Config" for topic creation. The controller class exposes an endpoint to create orders, while the OrderProducer class sends order details to the Kafka topic.

### Stock Service

The "Stock Service" module handles order consumption. The OrderConsumer class reads messages from the Kafka topic and registers order details in a MySQL database. This demonstrates how event-driven architecture maintains data consistency across microservices.

### Email Service

The "Email Service" module showcases another dimension of event-driven communication. The OrderConsumer class in this module receives order data from the topic and sends email notifications to customers, enhancing the user experience.

## Setup and Configuration

Before you begin, ensure that Spring Boot and Kafka are properly configured. Verify the necessary dependencies and configurations to ensure a smooth execution.

## Conclusion

The **Event-Driven Microservices Project** showcases the power of event-driven architecture in microservices communication. By implementing order processing and communication across different modules, we highlight how Spring Boot and Kafka enable us to build responsive and scalable systems. We encourage you to explore, experiment, and implement these concepts in your own projects.

#SpringBoot #Kafka #Microservices #EventDrivenArchitecture #Java #Scalability #GitHub
