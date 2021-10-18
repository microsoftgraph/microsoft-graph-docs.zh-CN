---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b371969e349340264b2a3ccd81ce008a1716b0c3
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450205"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知。|
|compliant|1|兼容。|
|不符合|2|设备不兼容，并且被阻止访问公司资源。|
|conflict|3|与其他规则冲突。|
|error|4 |错误。|
|inGracePeriod|254|设备不合规，但仍有权访问公司资源|
|configManager|255|由配置管理器管理|



