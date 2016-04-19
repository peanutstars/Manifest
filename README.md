# blah blah for Manifest

This manifest files are entry point for test, habit and share projects.


### Usage repo tool.

##### Download project

```shell
#> mkdir prj_folder
#> repo init -u https://github.com/peanutstars/manifest.git -m manifest_file.xml
#> repo sync
```

##### Prepare to push source upstream

###### Step #1
It refers to http://stackoverflow.com/questions/14540262/how-does-git-push-work-with-androids-repo-tool?answertab=active#tab-top .
```shell
#> repo start master [--all |<inner_project>...]
```

###### Step #2
Change, Modify, Delete and Add Codes and then push source upstream.
It could lost worked source codes, if it does not perform the STEP #1.
```shell
#> repo forall -c git commit -m "Comment for worked source"
#> repo forall -c git push github
```
