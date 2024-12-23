# React 19 useEffect Dependency Array Bug

This repository demonstrates a common error related to the useEffect hook in React 19.  Improper use of the dependency array can lead to unexpected behavior and difficult-to-debug issues. The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected version. 

## Problem
The issue stems from omitting necessary state variables within the useEffect hook's dependency array. This results in stale closures, causing the effect to not update correctly when its dependencies change.