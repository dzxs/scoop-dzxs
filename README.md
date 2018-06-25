## scoop-dzxs [![Build status](https://ci.appveyor.com/api/projects/status/0efmivy9k38cc3ae?svg=true)](https://ci.appveyor.com/project/dzxs/scoop-dzxs)

#### 安装 scoop 到自定义目录

```powershell
[environment]::setEnvironmentVariable('SCOOP','D:\Applications\Scoop','User')
$env:SCOOP='D:\Applications\Scoop'
iex (new-object net.webclient).downloadstring('https://raw.githubusercontent.com/lukesampson/scoop/master/bin/install.ps1')
```
#### 添加scoop-dzxs
```powershell
scoop bucket add dzxs https://github.com/dzxs/scoop-dzxs
scoop bucket list # -> you should see 'dzxs'
```

