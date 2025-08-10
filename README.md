# Desmos-Graphs

Javascript code to get number of bytes:

function getDesmosGraphByteSize(graph) {
  const jsonStr = JSON.stringify(graph);
  return new TextEncoder().encode(jsonStr).length;
}
const graphState = Calc.getState(); 
console.log(getDesmosGraphByteSize(graphState), "bytes");