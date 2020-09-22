---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 24f7a2a62ae45504c03d2fcff49ca8f17bfab28b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091304"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|合格|1 |合格.|
|合规|2 |设备不合规，并将从公司资源中阻止。|
|冲突|第三章|与其他规则冲突。|
|error|4 |错误。|
|inGracePeriod|254|Device 不合规，但仍有权访问公司资源|
|configManager|255|由配置管理器管理|









