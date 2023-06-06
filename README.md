# taoxanh.github.io

**to craft response and auto upload you will need** 
- jq
- gh
- unzip
- git

To upload rom and generate json simply run 
```source release.sh ../path/to/lineageos.zip```

if you want to host this on your own git you can change ```URL=``` value inside of ```release.sh```

On device side changes either add overlay for `updater_server_url`or add prop ```lineage.updater.uri```  that points to json 
e.g. ```lineage.updater.uri=https://raw.githubusercontent.com/taoxanh19999/taoxanh.github.io/main/17.1/{device}.json```

do note you can either hardcode {device} or leave it to updater to handle that tho in that case user might break otas by changing props
