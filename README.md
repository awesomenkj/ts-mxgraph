# A Tiny Typescript Wrapper for mxgraph

## Overview

A tiny wrapper around [mxgraph](https://github.com/jgraph/mxgraph-js) that
provides a configurable TypeScript compatible package.

## Usage
```sh
npm i -D ts-mxgraph
```

```typescript
import { mxgraph, mxgraphFactory } from "ts-mxgraph";

const { mxGraph, mxGraphModel } = mxgraphFactory({
    mxLoadResources: false,
    mxLoadStylesheets: false,
});

const container = document.getElementById("mxgraph-container");
if (container) {
    const model: mxgraph.mxGraphModel = new mxGraphModel();
    const graph: mxgraph.mxGraph = new mxGraph(container, model);
}
```

## License

[Apache 2.0 License](LICENSE)
