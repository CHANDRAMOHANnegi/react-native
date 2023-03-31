Virtual DOM has the same properties that of the Real DOM, but it lacks the power to directly change the content of the screen.


So when there is a update in the virtual DOM, react compares the virtual DOM with a snapshot of the virtual DOM taken right before the update of the virtual DOM.

With the help of this comparison React figures out which components in the UI needs to be updated. This process is called diffing. The algorithm that is used for the diffing process is called as the diffing algorithm.



COMPARISON betwon old virtual dom (Before updation) and new Virtual dom (After updation)  to figure out difference is DIFFING.



Virtual DOM is synced with real DOM with ReactDOM library. This process is called Reconciliation.


RECONCILIATION is the process through which React updates the Browser DOM.