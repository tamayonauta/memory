# General scripts

## Delete all migrations of a Django project

```sh
find . -path "*/migrations/*.py" -not -name "__init__.py" -delete
```

## Export git commits

```sh
git log --since="<date>" --author="<email or name>" --reverse --pretty=format:"%h,%an,%ar,%s" > <filename>
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

## Copy content from a file

### UNIX

```sh
pbcopy < <filename>
```

Example:

```sh
pbcopy < git-logs.txt
```