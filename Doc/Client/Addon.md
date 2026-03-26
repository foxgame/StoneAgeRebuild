# Addon模块，插件脚本模块，基本兼容老的STW、SAXP等外挂脚本。

## 语法
```xml
    <step moveMap="5106" moveX="20" moveY="36" /> 地图移动
    <step moveMap="5106" moveX="19" moveY="36" />
    <step itemHavePos="0" itemHave="飞行至达" jumpOK="OKDN" /> 检测道具
    <step flag="ABC" /> 标记
    <step moveMap="5106" moveX="16" moveY="13" />
    <step npcX="16" npcY="12" npcBuy="1" npcBuyNum="1" /> npc对话
    <step delay="0.500000" /> 延迟
    <step moveMap="5106" moveX="17" moveY="17" />
    <step itemHavePos="0" itemHave="行至达那" jumpNo="ABC" />
    <step moveMap="5106" moveX="19" moveY="23" />
    <step flag="OKDN" />
    <step moveMap="5106" moveX="19" moveY="29" />
    <step flag="测毛1" />
    <step itemHavePos="0" itemHave="福尔" jumpOK="OK" />
    <step talk="你的道具栏中没有福村羽毛，请准备好之后再继续脚本" />
    <step pause="1" /> 暂停
    <step jump="测毛1" /> 跳转
    <step flag="OK" />
    <step itemEmpty="4" jumpOK="OK2" /> 
```

## 快速使用
- 具体可参考游戏目录 Mods/addon1/Data/Addon/quest/xxx.xml 相关插件脚本

## 发布，需要配合Mod进行发布，参考[Mod](../Common/Mod.md)
