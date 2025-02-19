# Next.js 15: next/font TypeError in Server Components with Dynamic Imports

This repository demonstrates a rather uncommon bug in Next.js 15 related to using the `next/font` package with server components and dynamic imports.  The bug results in a runtime `TypeError` stating a function is undefined, even with seemingly correct import statements.  The issue is specifically triggered when dynamically importing a font within a server component that is itself dynamically imported.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Observe the error in the browser console or the terminal during the server-side rendering process.

## Solution

The provided solution file addresses the problem by restructuring the import and usage of the font, ensuring it's correctly available during server-side rendering.