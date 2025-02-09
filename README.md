# React Native Unhandled Network Error Example

This repository demonstrates a common issue in React Native applications: inadequate handling of network errors during data fetching.  The `DataFetch.js` file shows an example of fetching data from an API.  The issue is that while it handles the `response.ok` check it does not handle other potential network errors (like timeouts) effectively.  The solution in `DataFetchSolution.js` demonstrates a more robust approach.

## Problem

The original code catches errors during the fetch, but its error handling is minimal, potentially leaving the user with a confusing or non-informative message.  The application may not always gracefully handle things like network timeouts or other unexpected HTTP status codes.

## Solution

The improved version provides more specific and informative error handling, offering a better user experience in case of network problems.  It also demonstrates using a timeout to prevent indefinite blocking.
