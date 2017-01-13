# surgeConf2yaml
将`surge`的配置文件转位`yaml`格式的配置文件，供`SpechtLite`使用

> 目前会自动生成以下六个文件（如果配置文件不存在对应的内容，会自动创建空白文件）


* directlist
* directiprange
* proxylist
* proxyiprange
* rejectlist
* rejectiprange

## cd到下载后的可执行文件路径

```
$ cd /path/to/surgeConf2yaml
```
## 给予执行权限

```
$ chmod +x surgeConf2yaml
```

## 执行
参数 
> `-p` 表示 `surge` 的配置文件路径
> `-o` 表示输出到哪个目录下（可选），默认输出到`~/.SpechtLite`
> `-y`表示需要导出注释的行到文件
> `-f`表示会覆盖原来的文件（可选），默认不覆盖文件

```
$ ./surgeConf2yaml -p /path/for/surge.conf -o /path/to/output -y
```

## 已知问题
当配置文件最后一行没有回车时，无法读取该行


