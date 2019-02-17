# 实战篇2：开发一个清除缓存插件

本节我们开始写一个有真正用途的普通插件。

为了节省 TTS 消耗的时间，wukong-robot 支持将语音文件缓存到 `temp` 目录，但是如果时间久了，整个目录里的文件数量就会越来越多，大量占用设备的存储空间；此外，如果修改了 TTS 配置改了发音人的音色，如果没有清理已有的缓存语音，也会出现 wukong-robot 使用过程中混杂着多种音色的奇怪体验。所以，我们可以开发一个插件，来帮助清除缓存。

?> “缓存 LRU 自清理”是后面计划要做一件事：自动淘汰删除久未使用的缓存，就可以将缓存目录控制在一定的体积以内，避免造成过多的空间浪费。在这个功能完成之前，你可以[关注项目的进展](https://github.com/users/wzpan/projects/1)查看这个功能的实现进度，或者[帮助我实现它](https://github.com/wzpan/wukong-robot#%E8%B4%A1%E7%8C%AE)。

（未完待续）