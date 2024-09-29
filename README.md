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
5. Additionally you can type the name of the directory you want to be commited and pushed like so (where ~/Desktop/whatever-dir/ is replaced with the path to whatever dir you wanna have commited, 
and pushed)

```
qcom ~/Desktop/whatever-dir/
```

## Adding a message
You can also use the flag -m if you want to specify a different msg than the default "qcom"

```
qcom -m "changed xyz"
```
(works with previous dir option too)
```
qcom ~/Desktop/whatever-dir/ -m "changed xyz"
```

6. I would advise you set up githib push to work with ssh keys just to make everything easy

## TLDR Usage
$ qcom [optional directory] [optional flag -m] [message if using -m]

# CC BY-SA 4.0

