# QCOM: an auto committing and pushing tool to update repos quick and dirty (Linux)

## TLDR Usage

```
qcom [optional directory]
```

## Motivation
Sometimes you just want whatever code/configs/whatever inside a directory committed and pushed to github quick

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
sudo mv qcom /usr/local/bin

```

4. Go into a directory that you already have a git repo in that's setup to push to like github or another place and type
```
qcom
```
5. Additionally you can type the name of the directory you want to be commited and pushed like so (where ~/Desktop/whatever-dir/ is replaced with the path to whatever dir you wanna have commited, 
and pushed)

```
qcom ~/Desktop/whatever-dir/
```


6. I would advise you set up github push to work with ssh keys just to make everything easy and quick


## CC BY-SA 4.0

