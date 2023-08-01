# CoinApp - Android Project

CoinApp is an Android application that allows users to see the listing of different virtual coins available in the market and check the details of each coin. The main purpose of this project is to implement the Clean Architecture with Jetpack Compose using Hilt for dependency injection. It utilizes UseCases for business logic and fetches data from the Coinpaprika API.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Setup](#setup)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Clean Architecture](#clean-architecture)
- [Coinpaprika API](#coinpaprika-api)
- [License](#license)

## Introduction

CoinApp is a simple Android application that enables users to explore the virtual coins available in the market. Users can view a listing of various coins and get detailed information about each coin, such as its current price, market cap, and trading volume. The app follows the principles of Clean Architecture, making it maintainable, scalable, and testable. It uses Jetpack Compose for a modern and declarative UI, and Hilt for dependency injection to manage and provide dependencies.

## Features

- View a listing of different virtual coins available in the market.
- Check detailed information about each coin, including its current price, market cap, and trading volume.

## Setup

To run the CoinApp project locally, follow these steps:

1. Clone the repository: `git clone https://github.com/mehsan-dev/CoinApp.git`
2. Open the project in Android Studio.
3. Make sure you have the latest Android SDK and necessary build tools installed.

## Dependencies

The CoinApp project uses the following major dependencies:

- AndroidX: A collection of libraries that help you build robust and efficient Android apps.
- Jetpack Compose: A modern toolkit for building native Android UI with a declarative approach.
- Hilt: A dependency injection library for Android that reduces boilerplate code and simplifies dependency management.
- Retrofit: A type-safe HTTP client for Android and Java that makes API calls easy and efficient.
- Coinpaprika API: An API service to fetch virtual coin data.

For a complete list of dependencies and their versions, please refer to the `build.gradle` files in the project.

## Usage

The CoinApp offers the following functionalities:

1. **Coin Listing**: Users can view a list of different virtual coins available in the market. Each coin will display basic information like its name, symbol, and current price.

2. **Coin Details**: By tapping on a specific coin from the listing, users can access more detailed information about the coin. This includes its current price, market cap, trading volume, and other relevant data.

## Clean Architecture

The CoinApp follows the principles of Clean Architecture to maintain separation of concerns and make the codebase more maintainable, scalable, and testable. It is structured into the following layers:

- **Presentation Layer**: Contains the UI components (Activities, Fragments, etc.), ViewModels, and other UI-related logic using Jetpack Compose.
- **Domain Layer**: Defines the business logic and use cases of the app. It contains the Interactors or Use Cases that implement the app's business rules.
- **Data Layer**: Handles data sources, repositories, and data mapping. It includes the implementation of the Coinpaprika API client.

## Coinpaprika API

The CoinApp fetches data from the Coinpaprika API, which provides information about different virtual coins available in the market. The app uses Retrofit to make API calls and retrieve the required data.
