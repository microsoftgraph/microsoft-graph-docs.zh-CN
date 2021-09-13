---
title: complianceState 枚举类型
description: 合规性状态。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 051cc43f82dc1ed9a2e1155778eb111387219b86
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111017"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

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



