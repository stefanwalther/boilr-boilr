### Download the template

```
$ boilr template download {%=repository%} <template-tag>
```

### Fork, modify locally and save it

```
$ git clone {%=repository%}
```

cd into it, then

```
$ boilr template save $(PWD) <template-tag>

# e.g. 
$ boilr template save $(PWD) {%=name%}
```

if you have for force the local updates, use

```
$ boilr template save $(PWD) <template-tag> -f
```

### Use it

```
$ boilr template use {%=name%} .
```

### Get all templates

Get a list of all - locally installed - templates:

```
$ boilr template list
```