# Wark

This is a repository for storing useful assets

Anyone can reference the files of this warehouse or Fork them themselves

If there are CSS files or assets that you think are very useful and this warehouse is not included, please pull PR or raise an Issue

```bash
local repo = get-repo github.com:0xarch/Wark
if [ repo --not-included $file_you_think_useful ]; then
    if [ you can-raise-issue -eq 'true' ]; then
        repo --raise-issue $(your-brain get-text-about $file_you_think_useful)
        echo "Oh I'm fxxking good"
    else
        repo --pull-request $file_you_think_useful
    fi
else
    repo --raw-file $(repo --get-path $file_you_think_useful)
fi
```