# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router Dom v6.  The catch-all route unintentionally overrides other routes, even when a specific path matches.

The problem is caused by the order of routes within the `<Routes>` component. The catch-all route should always be placed last to ensure it only handles paths that don't match any other routes.