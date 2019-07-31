---
title: complianceState 枚举类型
description: 合规性状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6fff27abba5bce945b1f8abd74e94e2060114b17
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000016"
---
# <a name="compliancestate-enum-type"></a>complianceState 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

合规性状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|合格|1|合格.|
|合规|双面|设备不合规, 并将从公司资源中阻止。|
|冲突|第三章|与其他规则冲突。|
|error|4|错误。|
|inGracePeriod|254|Device 不合规, 但仍有权访问公司资源|
|configManager|255|由配置管理器管理|





