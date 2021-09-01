---
title: defenderCloudBlockLevelType 枚举类型
description: 云阻止级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d5f3133f21d9da39cd3cd7bd6bb34f693b85889d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805750"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

云阻止级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值，使用默认Windows Defender 防病毒阻止级别并提供强检测，而不会增加检测合法文件的风险|
|high|1|High 应用强级别的检测。|
|highPlus|2|High + 使用高级别，并应用其他保护措施|
|zeroTolerance|3|零容限阻止所有未知可执行文件|



