# MyLims

> Laboratory information management system for any kind of scientific field

## Database

Each element that describes somehow the visual interface and relates an
importance of a notebook is stored as a class. The relations between the classes
look like this:

[![Database proposal][db_proposal]][db_editable]

Has to be taken in account that the selected database is a NoSQL database,
therefore the classes don’t have to be in different collections and that all the
rules of normalization don’t apply to this case.

Each one of this classes can be described as following:

- **Experiment**: Wrapper that describes the relation between samples,
  conclusions based on the results, etc.
- **Sample**: The object that is studied, for example the wafer, device or chip
- **Measurement**: Measurement made to a sample, this can be an image, an
  electrical characterization, etc.
- **Analysis**: A process that generated new information based on the data of a
  measurement or several measurements, this could be the average of the values,
  a standard deviation, annotations on an image, etc.
- **Kind**: Fields of a given measurement. This schema defines the required
  fields and how are going to be saved in the measurement collection, but at the
  same time allows the frontend to know how to correctly visualize this values.
- **Components**: A list of elements that are going to describe visually the
  process, results, conclusions, notes, etc.

For a more detailed implementation please check the [`schemas definition`](./schemas)

## Community

- [MIT License](.LICENSE)
- [How to contribute?](CONTRIBUTING.md)
- [Code of conduct](CODE_OF_CONDUCT.md)

[db_proposal]: ./docs/db_proposal.png
[db_editable]: https://drive.google.com/file/d/124ZshwQydHyD_vGyoN6vkqrXGBr860uv/view?usp=sharing
