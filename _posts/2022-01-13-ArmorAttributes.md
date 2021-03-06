---
title: 护甲原理
tags:
  - Minecraft
---

<br>

# 翻译自 *fandom wiki* 的 [Armor](https://minecraft.fandom.com/wiki/Armor), 加上了自己的理解
## by Baioretto

<br><br><br>

# Mechanics
当一件护甲护甲为玩家吸收伤害时, 盔甲自身就会受损, 其耐久就会减少, 当吸收到一定量的伤害, 盔甲会完全的损坏.

注意如果伤害不是被盔甲自身吸收的, 而是被一个盔甲的保护类附魔所吸收, 盔甲就不会受损. 附魔也可以减少正常情况下盔甲不会减少的伤害.

<br>

## Damage type
以下的伤害类型被减少自盔甲, 并在最后损伤盔甲自身.
- 来自怪物与玩家的直接(近战)攻击.
> - 这包含力量与虚弱效果(effects)与伤害增加附魔(enchantments).
- 被箭矢, 潜影贝的弹丸或者被投出的三叉戟击中.
> - 这包含附魔的额外伤害(除了潜影贝的弹丸).
- 被恶魂或烈焰人的弹丸击中, 或被火球击中.
- 守护者或远古守护者的激光束.
- 来自荆棘附魔的伤害, 或者守护者和远古守护者的尖刺(弹反).
- 接触破坏性的块(火、熔岩、岩浆块、仙人掌或甜浆果丛).
- 摸河豚.
- 爆炸.
- 配方中至少有一颗烟花之星的烟花.
- 闪电.
- 被落下的铁砧击中.
- 被一个玩家或雪傀儡的雪球击中.
- 被一个玩家的鸡蛋击中.

以下的伤害类型不被减少自盔甲, 对盔甲自身没影响.
- 摔落伤害(包括末影珍珠，但保护和跌落保护附魔会降低摔落伤害)
- 着火造成的持续伤害.
- 在一个方块内窒息或由于实体推挤(包括世界边界).
- 溺水(部分是龟壳头盔).
- 饥饿。
- 鞘翅飞行时与方块相撞。
- 触摸篝火块.
- 魔术(唤魔者尖牙, 来自伤害药水或龙息的状态效果与瞬间伤害)(但保护附魔会减少魔法伤害).
- 坠入虚空或/kill.
- 在细雪块里面.
> - 这不包括玩家或怪物是否穿着任何皮甲.

<br>

## Defense points
护甲防御点由属性 `generic.armor` 控制.
玩家当前的防护等级由护甲条直观地表示.
盔甲计量表受所穿戴的特定部件以及盔甲等级的影响.
下表显示了每件盔甲默认添加的防御点数,以及全套盔甲为每种材料添加的总点数.

| 材料   | 全部装备          | 头盔 / 帽子  | 胸甲 / 外衣      | 护腿 / 裤子    | 靴子       |
|------|---------------|----------|--------------|------------|----------|
| 鞘翅   | 2 (🛡)        | 2 (🛡)   | N/A          | N/A        | N/A      |
| 皮革   | 7 (🛡🛡🛡🛡)  | 1 (🛡)   | 3 (🛡🛡)     | 2 (🛡)     | 1 (🛡)   | 
| 金    | 11 (🛡 × 5.5) | 2 (🛡)   | 5 (🛡🛡🛡)   | 3 (🛡🛡)   | 1 (🛡)   |
| 锁链   | 12 (🛡 × 6)   | 2 (🛡)   | 5 (🛡🛡🛡)   | 4 (🛡🛡)   | 1 (🛡)   |
| 铁    | 15 (🛡 × 7.5) | 2 (🛡)   | 6 (🛡🛡🛡)   | 5 (🛡🛡🛡) | 2 (🛡)   |
| 钻石   | 20 (🛡 × 10)  | 3 (🛡🛡) | 8 (🛡🛡🛡🛡) | 6 (🛡🛡🛡) | 3 (🛡🛡) |
| 下届合金 | 20 (🛡 × 10)  | 3 (🛡🛡) | 8 (🛡🛡🛡🛡) | 6 (🛡🛡🛡) | 3 (🛡🛡) |

不同的盔甲组合提供不同程度的防御.

<br>

## Armor toughness
在 Java 版中, 盔甲可以通过一个次属性 `generic.armor_toughness` 进一步保护玩家.
通常, 护甲可以抵消造成较大伤害的攻击的较小部分伤害.
护甲韧性抵抗这个效果, 减轻强力攻击的威力.
默认情况下, 只有钻石和下界合金盔甲提供韧性, 每件钻石盔甲提供2点韧性, 下界合金盔甲提供3点韧性.

| 材料   | 全部装备         | 头盔 / 帽子  | 胸甲 / 外衣  | 护腿 / 裤子  | 靴子       |
|------|--------------|----------|----------|----------|----------|
| 鞘翅   | 0 (🛡)       | 0 (🛡)   | N/A      | N/A      | N/A      |
| 皮革   | 0 (🛡)       | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   |
| 金    | 0 (🛡)       | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   |
| 锁链   | 0 (🛡)       | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   |
| 铁    | 0 (🛡)       | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   | 0 (🛡)   |
| 钻石   | 8 (🛡🛡🛡🛡) | 2 (🛡)   | 2 (🛡)   | 2 (🛡)   | 2 (🛡)   |
| 下届合金 | 12 (🛡 × 6)  | 3 (🛡🛡) | 3 (🛡🛡) | 3 (🛡🛡) | 3 (🛡🛡) |

不同的盔甲组合提供不同等级的盔甲韧性.

<br>

## Damage protection

受到的伤害取决于防御点数(defense points), 所穿盔甲的韧性(toughness)和攻击强度.

![](/assets/image/posts/2022-01-13-ArmorAttributes/damagedstat.png)

(注意: min和max操作符的意思是只使用它们后面的两个表达式(用逗号分隔)的最小或最大输出.
例如“y = min (2x, 16)”表示“y”是 等于“2x”和“16”中的最小值, 而忽略最大值.)

拆分后, 这意味着每个护甲点对来袭的一点(一点生命值)攻击提供 4% 的最大伤害减免(damage reduction).
在没有韧性的情况下, 每次来袭的一点攻击都会降低 2 个百分点的最大伤害减免.
2个防御点数(defense points)相当于8%的保护, 所以护甲可以达到的总保护值是80%,
钻石和下界合金套保护玩家免受 80% 的伤害, 铁提供 60% 的伤害减免, 皮革提供 28% 的伤害.

一件钻石盔甲(提供 +2 韧性)将 减少每次来袭的一点攻击的防御降低值 (降低 **_每次来袭的一点攻击_**的**_防御降低_** "defense reduction", 并不是**_伤害减免_** "damage reduction") 降低到 1.6%.

两件减少到 4⁄3% (约 1.3333%), 三件减少到 8⁄7%(约 1.1428%), 四件减少到 1%.
下界合金盔甲进一步减少了 每次来袭的一点攻击的防御降低值.

一件下界合金盔甲将 每次来袭的一点攻击的防御降低值 减少至 16⁄11% (约 1.4545%),
两件将其降低至 8⁄7% (约 1.1428%), 三件将其降低至 16⁄17% (约 0.9412%), 四个将其降低到 0.8%.
防御减免百分比减少的确切公式是: 

![](/assets/image/posts/2022-01-13-ArmorAttributes/defensereduction.png)

简单说, 随着韧性的增加, 高伤害攻击造成的防御降低量减少,
而随着韧性接近高值(通过命令), 高伤害攻击造成的防御降低变得可以忽略不计.
护甲的最终伤害减免值, 下限为每个护甲防御点减伤至少 0.8%, 总上限为 80%. 
如果护甲被修改成下限大于上限, 则忽略下限.
下面给出了护甲减少的说明.

![](/assets/image/posts/2022-01-13-ArmorAttributes/damagereduction.png)

![](/assets/image/posts/2022-01-13-ArmorAttributes/receiveddamage.png)

以表格形式(韧性为 0), 受到的伤害为:

| Armor / Attack damage | 1    | 2    | 3    | 4     | 5     | 6	    | 7	    | 8	    | 9	    | 10 	  | 11            | 12     | 	13   | 14     | 15    | 16    | 17     | 	18    | 	19   | 	20   |
|-----------------------|------|------|------|-------|-------|-------|-------|-------|-------|-------|---------------|--------|-------|--------|-------|-------|--------|--------|-------|-------|
| 0	                    | 1.00 | 2.00 | 3.00 | 	4.00 | 5.00	 | 6.00	 | 7.00	 | 8.00	 | 9.00	 | 10.00 | 11.00         | 12.00	 | 13.00 | 14.00	 | 15.00 | 16.00 | 17.00	 | 18.00	 | 19.00 | 20.00 |
| 1	                    | 0.98 | 1.98 | 2.98 | 	3.97 | 4.96	 | 5.95	 | 6.94	 | 7.94	 | 8.93	 | 9.92	 | 10.91         | 11.90	 | 12.90 | 13.89	 | 14.88 | 15.87 | 16.86	 | 17.86	 | 18.85 | 19.84 |
| 2	                    | 0.94 | 1.92 | 2.94 | 	3.94 | 4.92	 | 5.90	 | 6.89	 | 7.87	 | 8.86	 | 9.84	 | 10.82         | 11.81	 | 12.79 | 13.78	 | 14.76 | 15.74 | 16.73	 | 17.71	 | 18.70 | 19.68 |
| 3	                    | 0.90 | 1.84 | 2.82 | 	3.84 | 4.88	 | 5.86	 | 6.83	 | 7.81	 | 8.78	 | 9.76	 | 10.74         | 11.71	 | 12.69 | 13.66	 | 14.64 | 15.62 | 16.59	 | 17.57	 | 18.54 | 19.52 |
| 4	                    | 0.86 | 1.76 | 2.70 | 	3.68 | 4.70	 | 5.76	 | 6.78	 | 7.74	 | 8.71	 | 9.68	 | 10.65         | 11.62	 | 12.58 | 13.55	 | 14.52 | 15.49 | 16.46	 | 17.42	 | 18.39 | 19.36 |
| 5	                    | 0.82 | 1.68 | 2.58 | 	3.52 | 4.50	 | 5.52	 | 6.58	 | 7.68	 | 8.64	 | 9.60	 | 10.56         | 11.52	 | 12.48 | 13.44	 | 14.40 | 15.36 | 16.32	 | 17.28	 | 18.24 | 19.20 |
| 6	                    | 0.78 | 1.60 | 2.46 | 	3.36 | 4.30	 | 5.28	 | 6.30	 | 7.36	 | 8.46	 | 9.52	 | 10.47         | 11.42	 | 12.38 | 13.33	 | 14.28 | 15.23 | 16.18	 | 17.14	 | 18.09 | 19.04 |
| 7	                    | 0.74 | 1.52 | 2.34 | 	3.20 | 4.10	 | 5.04	 | 6.02	 | 7.04	 | 8.10	 | 9.20	 | 10.34         | 11.33	 | 12.27 | 13.22	 | 14.16 | 15.10 | 16.05	 | 16.99	 | 17.94 | 18.88 |
| 8	                    | 0.70 | 1.44 | 2.22 | 	3.04 | 3.90	 | 4.80	 | 5.74	 | 6.72	 | 7.74	 | 8.80	 | 9.90          | 11.04	 | 12.17 | 13.10	 | 14.04 | 14.98 | 15.91	 | 16.85	 | 17.78 | 18.72 |
| 9	                    | 0.66 | 1.36 | 2.10 | 	2.88 | 3.70	 | 4.56	 | 5.46	 | 6.40	 | 7.38	 | 8.40	 | 9.46          | 10.56	 | 11.70 | 12.88	 | 13.92 | 14.85 | 15.78	 | 16.70	 | 17.63 | 18.56 |
| 10                    | 0.62 | 1.28 | 1.98 | 	2.72 | 3.50	 | 4.32	 | 5.18	 | 6.08	 | 7.02	 | 8.00	 | 9.02          | 10.08	 | 11.18 | 12.32	 | 13.50 | 14.72 | 15.64	 | 16.56	 | 17.48 | 18.40 |
| 11                    | 0.58 | 1.20 | 1.86 | 	2.56 | 3.30	 | 4.08	 | 4.90	 | 5.76	 | 6.66	 | 7.60	 | 8.58          | 9.60	  | 10.66 | 11.76	 | 12.90 | 14.08 | 15.30	 | 16.42	 | 17.33 | 18.24 |
| 12                    | 0.54 | 1.12 | 1.74 | 	2.40 | 3.10	 | 3.84	 | 4.62	 | 5.44	 | 6.30	 | 7.20	 | 8.14          | 9.12	  | 10.14 | 11.20	 | 12.30 | 13.44 | 14.62	 | 15.84	 | 17.10 | 18.08 |
| 13                    | 0.50 | 1.04 | 1.62 | 	2.24 | 2.90	 | 3.60	 | 4.34	 | 5.12	 | 5.94	 | 6.80	 | 7.70          | 8.64	  | 9.62  | 10.64	 | 11.70 | 12.80 | 13.94	 | 15.12	 | 16.34 | 17.60 |
| 14                    | 0.46 | 0.96 | 1.50 | 	2.08 | 2.70	 | 3.36	 | 4.06	 | 4.80	 | 5.58	 | 6.40	 | 7.26          | 8.16	  | 9.10  | 10.08	 | 11.10 | 12.16 | 13.26	 | 14.40	 | 15.58 | 16.80 |
| 15                    | 0.42 | 0.88 | 1.38 | 	1.92 | 2.50	 | 3.12	 | 3.78	 | 4.48	 | 5.22	 | 6.00	 | 6.82          | 7.68	  | 8.58  | 9.52   | 10.50 | 11.52 | 12.58	 | 13.68	 | 14.82 | 16.00 |
| 16                    | 0.38 | 0.80 | 1.26 | 	1.76 | 2.30	 | 2.88	 | 3.50	 | 4.16	 | 4.86	 | 5.60	 | 6.38          | 7.20	  | 8.06  | 8.96   | 9.90  | 10.88 | 11.90	 | 12.96	 | 14.06 | 15.20 |
| 17                    | 0.34 | 0.72 | 1.14 | 	1.60 | 2.10	 | 2.64	 | 3.22	 | 3.84	 | 4.50	 | 5.20	 | 5.94          | 6.72	  | 7.54  | 8.40   | 9.30  | 10.24 | 11.22	 | 12.24	 | 13.30 | 14.40 |
| 18                    | 0.30 | 0.64 | 1.02 | 	1.44 | 1.90	 | 2.40	 | 2.94	 | 3.52	 | 4.14	 | 4.80	 | 5.50          | 6.24	  | 7.02  | 7.84   | 8.70  | 9.60  | 10.54  | 11.52	 | 12.54 | 13.60 |
| 19                    | 0.26 | 0.56 | 0.90 | 	1.28 | 1.70	 | 2.16	 | 2.66	 | 3.20	 | 3.78	 | 4.40	 | 5.06          | 5.76	  | 6.50  | 7.28   | 8.10  | 8.96  | 9.86	  | 10.80	 | 11.78 | 12.80 |
| 20                    | 0.22 | 0.48 | 0.78 | 	1.12 | 1.50	 | 1.92	 | 2.38	 | 2.88	 | 3.42	 | 4.00	 | 4.62          | 5.28	  | 5.98  | 6.72   | 7.50  | 8.32  | 9.18	  | 10.08	 | 11.02 | 12.00 |

请注意, 如果玩家穿着钻石盔甲或通过命令将韧性添加到盔甲上, 这些伤害值会降低.
如果不作弊, 在没有一件钻石或下界合金盔甲的情况下, 不可能获得 16 及以上的盔甲值(Defense points).

<br>

## Knockback reduction
每件下届合金盔甲给予 10% 的击退减少, 全套减少 40%