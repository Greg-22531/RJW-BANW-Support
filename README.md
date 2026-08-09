# RJW BANW Support

为 **BlueArchive-NewWorld（BANW）** 提供 RimJobWorld的兼容支持。

## 主要功能

### RJW 种族支持

- 将 BANW 学生（`BANW_KivotosStudent`）和老师（`BANW_KivotosSensei`、`BANW_Sensei_race`）注册为 RJW 可识别的种族。
- 为学生和老师补充 RJW 所需的身体部位，并启用性需求、生育与怀孕支持。
- 包含 BANW 身体贴图层级、服装遮挡和种族服装限制的兼容修正。

### 新生儿种族规则

本模组会覆盖 RJW Menstruation 对以下组合的新生儿种族选择；结果不受其杂交种族设置影响。

| 父母组合 | 新生儿结果 |
| --- | --- |
| 学生/老师 × 学生/老师 | 普通人类殖民者（智人种） |
| 学生/老师 × 非 BA 种族 | 完全采用非 BA 一方的种族 |
| 两名非 BA 父母 | 本模组不干预，沿用其他模组或游戏原有规则 |

上述规则与父母性别无关：只要父母中恰好一方是学生或老师，孩子就采用另一方的种类。

### Biotech 基因与异种继承

启用 **Biotech DLC** 时，如果父母中恰好一方是学生或老师，本模组会让遗传系统把非 BA 一方视为双方的遗传模板。换句话说，系统会按“两个非 BA 对象彼此生育”的方式计算孩子的基因与异种，而不是把 BA 一方混入计算。

- 可遗传异种按照 RimWorld 原版规则继承。例如，学生/老师与污骸种生育时，结果按“两名污骸种生育”计算，孩子保持污骸种身份，而不是显示为混血种。
- 学生/老师内部生育时只强制新生儿种类为普通 `Colonist`。

如果未启用 Biotech DLC，与基因及异种有关的 XML 兼容内容不会加载；RJW 种族支持和新生儿种族选择仍可使用。

## 支持版本

- RimWorld 1.6

## 前置模组

- [Harmony](https://steamcommunity.com/sharedfiles/filedetails/?id=2009463077)
- [BlueArchive-NewWorld](https://steamcommunity.com/sharedfiles/filedetails/?id=3560667190)
- [RimJobWorld](https://www.loverslab.com/files/file/7257-rimjobworld/)
- [RJW Menstruation](https://gitgud.io/lutepickle/rjw_menstruation)

Biotech DLC 不是基础 RJW 支持的必需项，但只有启用该 DLC 时才会应用异种和基因继承功能。

## 建议加载顺序

1. Harmony
2. BlueArchive-NewWorld
3. RimJobWorld
5. RJW Menstruation
6. RJW BANW Support

如果同时使用 RJW Sexperience，请将本模组放在其后加载。

## 安装

将整个 `RJW-BANW-Support` 文件夹放入 RimWorld 的 `Mods` 文件夹。
