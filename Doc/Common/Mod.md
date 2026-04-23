# Mod模块。
- 客户端，可以修改游戏中任意资源。配置文件、宠物造型、插件脚本。
- 服务器，可以修改配置文件，专属服新增道具等。

# 目录结构
- 参考客户端Mods文件夹。Mods\xxx\
- modInfo.xml文件为mod信息。
- Data\ mod数据目录

# 客户端
- Configs\，客户端配置，参考Config，放入目录即可。
- Animstions\，动画文件，可以使用动画编辑器生成。bytes文件放入目录即可。
- BattleMaps\，战斗地图，可以使用地图编辑器生成。bytes文件放入目录即可。
- Maps\，地图文件，可以使用地图编辑器生成。bytes文件放入目录即可。
- Musi\，音乐文件，ogg格式文件放入目录即可。
- Sounds\，音效文件，wav格式文件放入目录即可。
- Textures\，贴图文件，地形、建筑、npc等。png文件放入目录即可。
- TexturesOther\，其他贴图文件，图标、头像等。png文件放入目录即可。
- Addon\，插件脚本，参考客户端，需要配置。

# 服务器
- Configs，服务器配置，参考Config，放入目录即可服务器启动时加载。会自动同步给客户端使用。
- Npcs，NPC配置，参考Config，放入目录即可服务器启动时加载。

# 语法

# 发布
- 目前客户端mod编辑器暂时不可用，联系客服发布。
- 自建服务器mod可以自行放入服务器Mods\目录下，并配置modActive.xml，同客户端语法相同。  <m id="mod id" />
  
