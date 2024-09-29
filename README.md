# QCOM: an auto commiting and pushing tool to update repos quick and dirty

## Motivation
Sometimes you just want whatever code/configs/whatever inside a directory commited and pushed to github quick

usually I find myself in this pattern

```
git add .
git commit -m "whatever msg idc"
git push
```
or 
```
cd ~/Desktop/whatever-dir/
git add .
git commit -m "whatever msg idc"
git push
```

these can both be replaced by
```
qcom
```
or 
```
qcom ~/Desktop/whatever-dir/
```


## How to use 

1. Download files

2. Go into the directory of downloaded files and open a terminal there

3. Type these commands in the terminal

```
sudo chmod +x qcom
sudo mv qcom /usr/bin

```

4. Go into an empty or populated directory you want to commit+push and type (if no previous .git repo it will make one and ask you to specify a location to push to)
```
qcom
```
5. Additionally you can type the name of the directory you want to be commited and pushed like so (where program-1/ is replaced with the path to whatever dir you wanna have commited, 
and pushed)

```
qcom program-1/
```

## Adding a message
You can also use the flag -m if you want to specify a different msg than "qcom"

```
qcom -m "changed xyz"
```
(works with previous dir option too)
```
qcom program-1/ -m "changed xyz"
```
