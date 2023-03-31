The React Native renderer goes through a sequence of work to render React logic to a host platform. This sequence of work is called the render pipeline and occurs for initial renders and updates to the UI state. 


The render pipeline can be broken into three general phases:

1. Render: React executes product logic which creates a React Element Trees in JavaScript. From this tree, the renderer creates a React Shadow Tree in C++.

2. Commit: After a React Shadow Tree is fully created, the renderer triggers a commit. This promotes both the React Element Tree and the newly created React Shadow Tree as the “next tree” to be mounted. This also schedules calculation of its layout information.

3. Mount: The React Shadow Tree, now with the results of layout calculation, is transformed into a Host View Tree.