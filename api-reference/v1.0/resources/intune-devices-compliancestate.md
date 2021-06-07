---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4bae464724712333c81b73bdcd23e57148655624
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757736"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性状态。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知。|
|compliant|1|兼容。|
|不符合|2|设备不兼容，并且被阻止访问公司资源。|
|conflict|3|与其他规则冲突。|
|error|4 |错误。|
|inGracePeriod|254|设备不合规，但仍有权访问公司资源|
|configManager|255|由配置管理器管理|




