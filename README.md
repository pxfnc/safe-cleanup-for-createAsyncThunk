# safe cleanup for `createAsyncThunk`

## Problem

When using `createAsyncThunk` and React's `useEffect` hook, StrictMode calls cleanup when the Component is mounted to re-execute the effect. I would expect the next pending action to be dispatched after the rejected action, but the pending action is dispatched before the rejected action.

## Solution

I haven't found the answer yet.
