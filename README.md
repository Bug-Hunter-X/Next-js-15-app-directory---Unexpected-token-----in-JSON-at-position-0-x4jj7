# Next.js 15 App Directory - Unexpected Token '<' in JSON at position 0

This repository demonstrates a common error encountered in Next.js 15's App Router:  `Unexpected token '<' in JSON at position 0`. This typically arises when a page renders HTML directly instead of returning JSON data in an API route.

## Problem

When using the App Router, API routes are expected to return JSON data.  Attempting to render HTML directly from a page that's not meant for client-side rendering can lead to this error.  The browser expects JSON but receives HTML causing the parser to throw the error.

## Solution

The solution is to ensure that your API routes return valid JSON. If you need to render HTML, that should be done from a page component intended for client-side rendering.