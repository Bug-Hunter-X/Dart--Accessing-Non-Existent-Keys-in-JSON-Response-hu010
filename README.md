# Dart: Handling Non-Existent JSON Keys

This repository demonstrates a common error in Dart when handling JSON responses from APIs: attempting to access a key that might not exist in the JSON data.  The `bug.dart` file contains code that throws an exception when encountering a missing key.  The `bugSolution.dart` file provides a corrected version that handles this situation gracefully.

## The Problem

The `bug.dart` file shows how easily an error can occur when you directly access a key in a JSON map without checking for its presence. If the key isn't found, a runtime exception is thrown. This can crash your app.

## The Solution

The `bugSolution.dart` file demonstrates how to safely access JSON keys. It uses the `containsKey` method to check if the key exists before accessing its value. If the key is not found, it uses a default value or handles the situation appropriately, preventing the runtime exception.
