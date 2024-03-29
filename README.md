# boilr-boilr

> A boilr template to create a boilr template.

---

## Purpose
A boilr template to create a boilr template.

The following files are generated:

```
.
|-- .editorconfig
|-- .gitignore
|-- .verb.md
|-- Makefile
|-- README.md
|-- docs
|   |-- author.md
|   |-- boilr-installation.md
|   |-- boilr-output-wrapper.md
|   |-- boilr-purpose.md
|   |-- boilr-usage.md
|   |-- contributing.md
|   `-- related.md
|-- package.json
|-- project.json
`-- template

2 directories, 14 files

```

## Installation
Install [boilr](https://github.com/tmrts/boilr) first. 

Then use 

```
$ boilr download stefanwalther/boilr-boilr <template-tag>
```

e.g.
```
$ boilr download stefanwalther/boilr-boilr boilr-boilr
```

## Usage
### Download the template

```
$ boilr template download stefanwalther/boilr-boilr <template-tag>
```

### Fork, modify locally and save it

```
$ git clone stefanwalther/boilr-boilr
```

cd into it, then

```
$ boilr template save $(PWD) <template-tag>

# e.g. 
$ boilr template save $(PWD) boilr
```

if you have for force the local updates, use

```
$ boilr template save $(PWD) <template-tag> -f
```

### Use it

```
$ boilr template use boilr-boilr .
```

### Get all templates

Get a list of all - locally installed - templates:

```
$ boilr template list
```

## About

### Related projects
Some related projects:

 

### Author
**Stefan Walther**

* [twitter](http://twitter.com/waltherstefan)  
* [github.com/stefanwalther](http://github.com/stefanwalther) 
* [LinkedIn](https://www.linkedin.com/in/stefanwalther/) 
* [qliksite.io](http://qliksite.io)

### License
MIT

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.8.0, on December 06, 2022._

