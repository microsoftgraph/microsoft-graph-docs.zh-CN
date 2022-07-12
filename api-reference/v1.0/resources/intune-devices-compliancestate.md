---
title: complianceState 枚举类型
description: 符合性状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 20d0c049a8274bbedf4c618c54cdf003b9fbfb63
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66736074"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

符合性状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|兼容|1|兼容。|
|不符合|2|设备不符合要求，并且被阻止使用公司资源。|
|冲突|3|与其他规则冲突。|
|error|4|错误。|
|inGracePeriod|254|设备不合规，但仍有权访问公司资源|
|configManager|255|由 Config Manager 管理|





