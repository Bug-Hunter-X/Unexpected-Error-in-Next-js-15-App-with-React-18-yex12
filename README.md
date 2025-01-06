# Next.js 15 Unexpected Error with React 18

This repository demonstrates a bug encountered in Next.js 15 when using certain React 18 features.  The issue involves unexpected behavior during rendering, leading to errors during build or runtime. The problem is related to how React 18's automatic batching interacts with Next.js's internal rendering processes.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.

Observe the error during development or when building the application.

## Solution

The solution involves carefully managing state updates and rendering within the Next.js app, potentially utilizing techniques such as `useCallback` or `useMemo` to prevent unintended re-renders.