A block diagram shows [[transfer functions]] as blocks and the flow of a signal with arrows. Typically a feed forward function block is represented with $G_{1,2,3...n}$ and a feedback function is represented with $H_{1,2,3...n}$ .

example : 
![[Block Diagrams and their simplification 2026-03-22 20.51.03.excalidraw]]
R(s) -> reference input
C(s) -> controlled output

## Simplification of Block diagram :
To simplify a complex block diagram means to reduce a complex block diagram with many blocks and summing points into a diagram with only 1 block, input and output, such that its easy to calculate the overall transfer function of the system

### Rules for simplifying a block diagram : 
1. If two or more blocks are in series (one after another), multiply them, and conversely if they're parallel, add them (basically capacitors). 
   **![[Block Diagrams and their simplification 2026-03-22 21.11.40.excalidraw]]** 
2. to move a summing point BEHIND a block, 