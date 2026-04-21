# Agent模块
- AI大模型驱动游戏，可以控制当前角色或其他角色行动。
- 理论上接入视觉模块后，可支持任意类型游戏。
- 实验性功能，**目前只支持PC平台**，不定期更新。

## 配置 config.xml：
``` xml
<root>
	<agent name="main" base="https://api.deepseek.com" key="" model="deepseek-chat" mode="main" />
	<agent name="map" bae="https://api.deepseek.com" key="" model="deepseek-chat" mode="function" />
	<agent name="player" base="https://api.deepseek.com" key="" model="deepseek-chat" mode="function" />
	<agent name="addon" base="https://api.deepseek.com" key="" model="deepseek-chat" mode="function" />
	<agent name="chat" base="https://api.deepseek.com" key="" model="deepseek-chat" mode="chat" />
	<agent name="story" base="https://api.deepseek.com" key="" model="deepseek-chat" mode="chat" />
</root>

```
- name="agent名称" base="AI模型地址" key="api key" model="AI模型" mode="返回模式"
- main，主模块，负责生成并分配任务
- function，负责子模块执行具体操作
- chat，聊天模块，负责输出信息
- story，攻略模块，负责查询攻略，**目前大模型基本无法满足需求，需要重新训练。**

## Memory/ 记忆目录

## Script/ 脚本目录
- player.lua player模块脚本，负责调用角色相关。
- addon.lua addon模块脚本，负责游戏脚本相关。
- map.lua map模块脚本，负责游戏地图相关。
- chat.lua chat模块脚本，负责游戏聊天相关。

## System/ Agent system目录
- main.md ，主模块system
- player.md ， player模块system
- map.md ， map模块system
- addon.md , addon模块system
- chat.md , chat模块system
- story.md , story模块system

## 实现原理
- 功能相对复杂，可联系开发者咨询
  
## 快速使用
- 申请大模型API KEY，修改config.xml key字段，默认需要五个模型，可根据情况自行添加
- /ai x ，初始化ai，加载agents。
- /a 指令，操作当前角色。/a 我要去xx村，AI会自动调用相关脚本操作。
- /a chat 指令，指定chat agent模块执行指令。/a chat 聊两句。
- 指挥其他角色，/r id，进入私聊模式，a:指令 需要对方已开启/ai

# 已支持的指令
- 去xx村
- 去xx挂机
- 查找xx脚本
- 查询当前位置
- 查询npc某某，返回当前地图某某信息
- 查询正在执行脚本。
- 查询多少石币
- 返回记录点
- 跟随指定玩家，或叫他过来我这里。
- 组队、离开队伍
- 去某某地挂到多少级。
- 去某某地把宠物挂到多少级。
- 执行某某脚本、停止执行脚本。
- 交易我多少石币、交易我某某道具等。（需要面对面、vip1）


## 效果展示
https://github.com/user-attachments/assets/05b953fe-c2e6-40fe-9cf9-eec178b03517

