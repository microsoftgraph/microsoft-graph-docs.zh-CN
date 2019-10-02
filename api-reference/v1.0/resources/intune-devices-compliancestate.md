---
title: complianceState 枚举类型
description: 合规性状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 01c0a3443eae87fb69b4b6482a2da2c2e067c5d1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357057"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|合格|1|合格.|
|合规|双面|设备不合规，并将从公司资源中阻止。|
|冲突|第三章|与其他规则冲突。|
|error|4|错误。|
|inGracePeriod|254|Device 不合规，但仍有权访问公司资源|
|configManager|255|由配置管理器管理|




