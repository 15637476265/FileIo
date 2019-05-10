# FileIo
FileIo Plus QML plugin
file io增强版
#使用方法
```
#INCLUDEPATH += "$$PWD\include"
#LIBS += "$$PWD\lib\FileIo.lib"
```

```
import plugins.FileIo 1.0


FileIO{
        id:fileIo
        source: ("file:///"+runPath+ "/conf/" + "conf.json")
        onSourceChanged: {
            fileIo.read()
        }
        onTextChanged: {
            //**todo
        }
    }
```
