# Zoo Simulation

A zoo built from a text file: animals, the enclosures that hold them, and the
keepers that look after them. Java Lessons, task 8.

## What it covers

- A deep inheritance tree - `Animal` to `Ape`/`BigCat` to `Gorilla`, `Chimpanzee`,
  `Lion`, `Tiger`, alongside `Bear`, `Elephant`, `Giraffe` and `Penguin`.
- Reflection: the zoo is populated from species names read out of a data file, so
  adding a species means adding a class, not editing a switch statement.
- Composition - `Enclosure`, `FoodStore` and the `Zookeeper` subclasses each own a
  slice of the simulation.
- Loading the zoo's state from text and writing it back.

## Running it

```bash
javac -d out $(find src -name "*.java")
java -cp out Simulation
```

## Layout

- `src/Animals/`, `src/Enclosures/`, `src/FoodStores/`, `src/Zookeepers/` - the model.
- `src/Data/zoo.txt` - the starting zoo; `myZoo.txt` is what a run writes back.
- `src/Simulation.java` - the entry point.
- `src/ZOO Spec.pdf` - the original task sheet.
