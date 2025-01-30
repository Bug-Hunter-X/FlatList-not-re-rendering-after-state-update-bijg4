# React Native FlatList Re-rendering Issue

This repository demonstrates a common issue in React Native where a FlatList component fails to re-render even when its data source (state) changes.  The example uses a simple FlatList to display a list of items. Despite the state updating correctly, the FlatList remains empty. This issue often arises due to improper key handling or missing dependencies in `useEffect` hooks.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` or `yarn install`.
3. Run the app on an Android or iOS emulator/device.
4. Observe that the FlatList remains empty.

## Solution

The solution involves ensuring that the `useEffect` hook has the correct dependencies and potentially adding a unique key prop to each list item. See `bugSolution.js` for the corrected code.