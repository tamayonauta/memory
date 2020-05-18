# Python commands

## Virtual Environment

- Create virtual environment

  ```sh
  python3 -m venv <venv_path>
  ```

  Example:

  ```sh
  python3 -m venv myenv
  ```

- Activate virtual environment

  ```sh
  source <venv_path>/bin/activate
  ```

  Example:

  ```sh
  source myenv/bin/activate
  ```

- Deactivate virtual environment

  ```sh
  deactivate
  ```

## Pytest

- Run tests without warnings

  ```sh
  pytest --disable-warnings
  ```

- Run tests with fail fast

  ```sh
  pytest -x
  ```

- Run tests watching full differences

  ```sh
  pytest -vv
  ```

- Run tests with print function

  ```sh
  pytest -s
  ```

- Run tests of a file or directory

  ```sh
  pytest <file_or_directory_path>
  ```

- Run tests with many options

  ```sh
  pytest -x -s -vv --disable-warnings
  ```
