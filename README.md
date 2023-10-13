# TheHive文档备份
TheHive4文档将在2023 年 12 月 31 日之后永久停用。备份如下：
TheHive:https://h4m5t.top/thehive_docs/thehive/
Cortex:https://h4m5t.top/thehive_docs/cortex/
By h4m5t.

## Test changes

```bash
# Install the requirements first
pip install -r requirements.txt

# Start the mkdocs server in development mode
mkdocs serve
```

Alternatively you can use a docker container:

```bash
docker build . -t thehive-docs
docker run -it --rm -p 8000:8000 -v $PWD:/docs thehive-docs
```

## Deploy

After commiting changes in `main`branch, deploy the documentation by running this command: 

```bash
mkdocs gh-deploy --remote-branch gh-pages
```
