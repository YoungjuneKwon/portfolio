# Open Source — statistics on the client

Two published npm packages, both MIT, both with CI and generated API docs.

## [@winm2m/inferential-stats-js](https://www.npmjs.com/package/@winm2m/inferential-stats-js)

A headless JavaScript SDK for SPSS-level inferential statistics that runs **entirely in the
browser**. No backend, no data leaving the machine.

The interesting constraint is that serious statistics live in the Python scientific stack, and
reimplementing them in JavaScript means reimplementing their numerical edge cases too — which is
exactly where a statistics library loses credibility. So the package runs the Python
implementations under WebAssembly via Pyodide and exposes them behind a typed TypeScript API.
Callers get JavaScript ergonomics and published numerical behaviour at the same time.

Coverage: descriptive statistics, compare means, regression, classification, dimension reduction,
and scale reliability. Progress events are surfaced so long analyses can report to the UI rather
than freezing it.

TypeScript 5.7 · Pyodide · Jest · TypeDoc · CITATION.cff for academic citation

## [@winm2m/react-stats-ui](https://www.npmjs.com/package/@winm2m/react-stats-ui)

React components for the workflows above — variable selection, test configuration, and
publication-formatted result tables — built on the SDK.

React 18/19 · TypeScript 5.5

## Why they are separate packages

Proveri needs both the computation and the interface, but the computation is useful on its own:
a researcher embedding one regression in a teaching page should not have to adopt a component
library. Splitting them also forces the SDK to have an API that is pleasant without the UI —
the fastest way to find out that an abstraction is wrong is to make something else depend on it.
