# Chapter Runloop

## Input

- current chapter source text
- `workspace/state/book_state.json`

## Output

- chapter truth JSON
- chapter retelling text
- chapter audit report
- chapter graph artifacts
- updated `book_state.json`

## Required order

1. read chapter
2. resolve aliases provisionally
3. extract truth
4. check must-keep coverage
5. generate retelling
6. update state
7. derive graphs
8. audit
9. freeze checkpoint

## Stop conditions

Do not advance if:

- audit blocks the chapter
- state continuity is broken
- truth is missing key causal information
