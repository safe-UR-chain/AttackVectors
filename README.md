# AttackVectorsTree
A web-based visualization of cyber security attack vactors.

## Update Mindmap

1. Download and open [Freemind]( https://freemind.de.softonic.com/ ).
2. Open the file `attack-vectors.mm` from the repositories` rot folder.
3. Use the function `Export > with XSLT` and select the `mm2json.xls` and the `attack-vectors.json` to transform the mindmap into a json tree.
4. Copy the entire content of `attack-vectors.json` into the `main.js` file located in the `assets/js` directory. Put the content into the returned object like shown below.

~~~~js
function getTree(rootName) {
    return {
      name: rootName,
      children: [
        // content of attack-vector.json goes here...
        ]
    };
}
~~~~
