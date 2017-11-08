#sublime text 3 安装插件
[Toc]
##安装插件
详细查看[官网](https://packagecontrol.io/installation#st2)
####Sublime Text3
`import urllib.request,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); urllib.request.install_opener( urllib.request.build_opener( urllib.request.ProxyHandler()) ); by = urllib.request.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); print('Error validating download (got %s instead of %s), please try manual install' % (dh, h)) if dh != h else open(os.path.join( ipp, pf), 'wb' ).write(by) `
####Sublime Text2
`import urllib2,os,hashlib; h = 'df21e130d211cfc94d9b0905775a7c0f' + '1e3d39e33b79698005270310898eea76'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://packagecontrol.io/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')`
##插件列表
我的插件列表(待补充)

##sublime运行php脚本
1. 将php添加到环境变量（或者配置php.exe的全路径）
2. 添加php的build system
    1. Tools->Build System->New Build System
    2. 弹出文件中修改为
    ```
    { 
    "cmd": ["php", "$file"],
    "file_regex": "php$", 
    "selector": "source.php" 
    }
    ```
        保存在默认的目录下即可，注意修改文件名为 php.sublime-build 。执行快捷键为`Ctrl+b`。
##添加代码片段
    Tools->New Snippet
##

