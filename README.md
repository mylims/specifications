# MyLims

> Laboratory information management system for any kind of scientific field

## Database

Each element that describes somehow the visual interface and relates an
importance of a notebook is stored as a class. The relations between the classes
look like this:

[![Database proposal][db_proposal]][db_editable]

Has to be taken in account that the selected database is a NoSQL database,
therefore the classes don’t have to be in different collections and that all the
rules of normalization don’t apply to this case. For a more detailed
implementation please check the [`schemas definition`](./schemas).

## Kinds

- [Measurements](./docs/project.md#measurements)

## Community

- [MIT License](.LICENSE)
- [How to contribute?](CONTRIBUTING.md)
- [Code of conduct](CODE_OF_CONDUCT.md)

[db_proposal]: ./docs/db_proposal.png
[db_editable]: https://drive.google.com/file/d/124ZshwQydHyD_vGyoN6vkqrXGBr860uv/view?usp=sharing
