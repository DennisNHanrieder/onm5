OMM Assignment 5 
Dennis Hanrieder s2210238022

Chatgbt Prombt: what is a radio group?
Chargbt Answer: 

A radio group is a set of options where only one can be selected at a time. It's commonly used when the user needs to pick one choice from a list.

🔘 Real-World Example:
Think about when you're filling out a form and see something like this:

Choose a filter:

( ) None

(•) Grayscale

( ) Sepia

( ) Blur

This is a radio group—each option is a radio button, and selecting one automatically deselects the others.

🧠 Why Use It?
Radio groups are perfect when:

You want to limit the user to one option.

The options are mutually exclusive (can't be combined).

You want a clear UI to show the current selection.

🧱 HTML Example:
html
Kopieren
Bearbeiten
<form>
  <label><input type="radio" name="filter" value="none"> None</label>
  <label><input type="radio" name="filter" value="grayscale"> Grayscale</label>
  <label><input type="radio" name="filter" value="sepia"> Sepia</label>
</form>
Notice how all radio buttons share the same name="filter"? That’s what groups them—so only one can be selected at a time.

🧩 In React
In React, you’d manage the selected option with state, like:

tsx
Kopieren
Bearbeiten
const [filter, setFilter] = useState("none")

<input type="radio" value="grayscale" checked={filter === "grayscale"} onChange={() => setFilter("grayscale")} />
Would you like to add a radio group for filter selection in your app too?
