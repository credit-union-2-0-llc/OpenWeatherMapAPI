# CODEBASE.md — credit-union-2-0-llc/OpenWeatherMapAPI

## Purpose
Legacy iOS library for fetching weather data from OpenWeatherMap. It is no longer under active development and serves as a historical reference rather than a maintained tool.

## Stack
Objective-C runtime targeting iOS. The codebase relies on standard Foundation frameworks and utilizes CocoaPods for dependency management (specifically version ~> 0.0.5).

## Entry Points
There are no executable entry points or CLI commands. Usage is intended via import: `#import "OWMWeatherAPI.h"` within an Objective-C iOS application.

## Key Directories
- Root directory contains the core `OWMWeatherAPI` implementation files.
- Example usage is demonstrated in `OWMViewController.m`.
- No subdirectories for tests or documentation are present.

## External Dependencies
Requires an active API key from [openweathermap.org](http://openweathermap.org/). The library acts as a wrapper for the OpenWeatherMap HTTP API, handling JSON parsing and language localization settings.

## Development Status
Inactive. The project is archived, and users are directed to alternative libraries such as SwiftOpenWeatherMapAPI or JFOpenWeatherMapManager for modern implementations.

## Gotchas
The API version (0.0.5) uses specific method naming conventions (e.g., `andCallback:` instead of `withCallback:` for daily forecasts). Temperature units default to Celsius but can be changed via `setTemperatureFormat`.