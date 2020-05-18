# General scripts

## Delete file or directory

- Delete all migrations of a Django project

  ```sh
  find . -path "*/migrations/*.py" -not -name "__init__.py" -delete
  ```

- Delete `__pycache__` files

  ```sh
  find . | grep -E "(__pycache__|\.pyc|\.pyo$)" | xargs rm -rf
  ```

## Content

- Clear content file

  ```sh
  echo -n "" > <file_name>
  ```

- Check differences between two files

  ```sh
  diff <file_name_1> <file_name_2>
  ```

- Copy content into the clipboard from a file

  ```sh
  pbcopy < <file_name>
  ```

  Example:

  ```sh
  pbcopy < git-logs.txt
  ```

## Git

- Export git commits

  ```sh
  git log --since="<date>" --author="<email or name>" --reverse --pretty=format:"%h,%an,%ar,%s" > <file_name>
  ```

  Example:

  ```sh
  git log --since="yesterday" --author="John Tamayo" --reverse --pretty=format:"- %s" > git-logs.txt
  ```

  ```sh
  git log --since="last week" --author="John Tamayo" --reverse --pretty=format:"- %s" > git-logs.txt
  ```

  ```sh
  git log --since="march 31 2019" --author="John Tamayo" --reverse --pretty=format:"- %s" > git-logs.txt
  ```

  ```sh
  git log --since="03-31-2019" --author="John Tamayo" --reverse --pretty=format:"- %s" > git-logs.txt
  ```
