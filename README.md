# Readme

## Remaining Issue - index.html line 52

Look the layouts/index.html

## older issue

When trying to get 
```
{{ $imagesrc := resources.Get .Params.coverImage }}
```
with a condition under the
```
{{ with .Params.Images }}
```
the Hugo output error:
```
execute of template failed at <.Params.coverImage>: can’t evaluate field Params in type []interface {}
```

This Does work with (solved)
```
{{ with $.Params.Images }}
```
This is now (solved) with below code
```
{{ with $.Params.Images }}
```
