# FileIo
FileIo Plus QML plugin
无需在main.cpp中注册
##file io增强版
##使用方法
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

##dll路径必须存放在   $$PWD\plugins\FileIo\FileIo.dll
