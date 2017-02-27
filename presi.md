class: center, middle

#Fast React

---

#Covers...

1. Intro
2. Basic Usage
  - Elements - ReactDOM
  - Components
3. State, Reconciliation, Component Architecture
4. Advantages
  - Metrics
  - Functional Programming

---

#Intro
- React was created to reduce complexity of managing state.
- React simply represents state of app with unidirectional data flow from state to presentation.
- No more templating. Just pure JavaScript objects, data types and functions.

---

# Basic Usage
Presentation

1. Elements/JSX
2. Creating Components and Inline Styles

---

#State
Unidirectional architecture
---

#Reconcitliation
(visual)

virtual DOM diffing

(notes)

The heart of React's performance is through the process in which it reconciles state changes. 
On every state change, the React virtual DOM is completely recreated from scratch and compares to the previous state of the virtual DOM, then writes the diff to the real DOM. So, it's a minimal write to the DOM and no reads. To expense of updates is reduced to only those writes.
JavaScript operations are cheap, reading/writing DOM is expensive. This reconciliation process reduces updates to the minimal necessary writes while reusing every other node.

---
#End