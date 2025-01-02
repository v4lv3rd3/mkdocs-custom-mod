# mkdocs-custom-mod
>[!Warning]
>I use `--break-system-packages` because im not using venv
## 1 - Install mkdocs
```shell
sudo apt update
sudo apt install python3 -y
sudo apt install python3-pip -y
pip install mkdocs --break-system-packages
```

## 2 - Clone the repo
```shell
git clone https://github.com/v4lv3rd3/mkdocs-custom-mod.git
```

## 3 - Install some packages

```shell
pip install mkdocs-material --break-system-packages
pip install "mkdocs-material[imaging]" --break-system-packages
sudo apt install libcairo2 libcairo2-dev -y
```

## 4 - Create and build the project

```shell
mkdocs new project-name
mv repo/* project-name
cd project-name
mkdocs build
mkdocs serve -a 0.0.0.0:1234 
```
