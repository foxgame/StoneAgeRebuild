# Config/ 配置表

### 通用配置：
- ban.csv 屏蔽配置
```csv
type(类型),data(屏蔽内容)
4,xxx
```
- battleMap.csv 战斗地图配置
- chat.csv 聊天相关配置
- creature.csv 怪物配置
```csv
name(名称),id,baseID,attack（攻击）,attackTarget（攻击目标）,attackAI（攻击AI）,defence（防御）,magic（魔法）,escape（逃跑）,wa0,wa1,wa2,wa3,wa4,wa5,wa6,rn,unknow,levelMin（最小等级）,levelMax（最大等级）,numMax（最大数量）,numMin（最小数量）,fight,exp,dp,type,pet（可捕捉）,item0（掉落道具）,item1,item2,item3,item4,item5,item6,item7,item8,item9,itemPro0（掉落概率）,itemPro1,itemPro2,itemPro3,itemPro4,itemPro5,itemPro6,itemPro7,itemPro8,itemPro9
初期拥有的乌力乌力,1,2,1,1,1,0,0,0,0,0,0,0,0,0,0,0,0,1,1,1,1,1,-1,-1,0,1,1234,1235,0,0,0,0,0,0,0,0,800,200,0,0,0,0,0,0,0,0
```
- creatureBase.csv 怪物基础配置
```
name(名称),id,initNum(初始属性点),levelUpPoint（升级成长）,baseVitality（基础体力）,baseStrength（基础力量）,baseToughness（基础耐力）,baseDexterity（基础敏捷）,ai,get,earth（地）,water（水）,fire（火）,wind（风）,poison（抗性）,paralysis,sleep,stone,drunk,confusion,petSkill0（技能）,petSkill1,petSkill2,petSkill3,petSkill4,petSkill5,petSkill6,rare,critical,counter,slot,animation,petFlag,size,atomBaseAdd0,atomFixMin0,atomFixMax0,atomBaseAdd1,atomFixMin1,atomFixMax1,atomBaseAdd2,atomFixMin2,atomFixMax2,atomBaseAdd3,atomFixMin3,atomFixMax3,atomBaseAdd4,atomFixMin4,atomFixMax4,limitLevel（等级限制）,amalgamation,material0（合成相关）,material1,material2,material3,material4
乌力,1,10,4.5,20,12,15,25,150,11,80,20,0,0,0,0,0,0,0,0,1,0,0,0,0,0,0,0,1,1,6,100250,1,0,0,700,700,0,700,700,0,700,700,0,700,700,0,700,700,0,0,0,1,2,3,4
```
- effect.csv 特效配置
- item.csv 道具配置
- itemCount.csv 道具叠加配置
```
```
- magic.csv 魔法配置
```
```
- map.csv 地图配置
- photo.csv 相册配置
- skill.csv 技能配置
```
```
- skillCode.csv 技能学习配置
```
```
- string.csv 文字相关配置
- texture.csv 贴图配置

### 客户端配置：
- audio.xml 声音相关配置
- help.xml 帮助配置
- quest.xml 任务配置

### 服务器配置：
- gameConfig.xml

```xml
<root>
	<base defalutStone="初始金币" maxLevel="最大等级" stone="携带石币" lp="升级点数" exp="经验倍率" fame="声望值" /> 
	<login map="初始地图id" x="东" y="南" />
	<auction sellRate="拍卖行手续费" />
	<battle ridePower="0.6" nono0="1.0" nono1="1.3" crit0="1.5" crit1="2.5" rideDown="0.7" rideDown0="0.6" rideDown1="0.8" dp="5" rand="0.15" stone="1.5" def="1.55" defp="1.35" batk="1.0" bdef="0.75" lv="0.4" min="0.16" >
		<b pet="251" atk="0.9" def="0.9" /> 战斗宠物伤害修正
 	</battle>
	<catch>
		<p pet="796" item="20247" num="1" /> 特殊捉宠道具
		<p pet="812" item="20292" num="1" />
	</catch>
	<onceQuest> 一次性任务
		<q id="69" />
		<q id="70" />
		<q id="71" />
		<q id="72" />
	</onceQuest>
	<guestData vit="20" str="20" tgh="20" dex="20" hp="140" mp="100" fire="100" lv="1" charm="59" /> 
	<trans questAdd="0.25" questCount="60" max="5" item="60020" v="0.1" s="0.1" t="0.1" d="0.1" stone="1000000" pet1="1373" pet2="1374" pet3="1375" pet4="1376" /> 转生相关
	<transPet v="0.1" s="0.1" t="0.1" d="0.1" vMin="0.1" sMin="0.1" tMin="0.1" dMin="0.1" vMax="1.2" sMax="0.46" tMax="0.46" dMax="0.46" dead="0.006" luck="0.011" vrMin="-0.3" vrMax="0.2" srMin="-0.14" srMax="0.15" trMin="-0.14" trMax="0.15" drMin="-0.14" drMax="0.15" /> 转宠相关
	<noTrade>
		<t pet="1610" /> 禁止交易宠物
	</noTrade>
	<noAuction>
		<t pet="1610" /> 禁止拍卖宠物
	</noAuction>
	<pet expItem="19549" br="0.4" bMin="4.5" bMax="4.89" r="0.2" rd="5" >
		<p pet="1558" lp="4.9" r="0.2" /> 特殊宠物成长修正
	</pet>
</root>
```

- enemyCount.csv 怪物数配置
```
```
- enemyGroup.csv 怪物组配置
```
```
- exp.csv 经验
```
```
- expEnemy.csv 怪物经验
```
```
- family.csv 家族配置
- gamble.csv 游乐场配置
- gambleItem.csv 游乐场道具配置
- mapWarp.csv 地图跳转配置
```
```
- mm.csv 宠物转生配置
- pvp.csv pvp配置
- question.csv 百人道场配置
- race.csv 游乐场竞速配置
- vip.csv vip配置
```
```
- vipShop.csv vip商店配置
```
```
- npc/ npc配置
  
