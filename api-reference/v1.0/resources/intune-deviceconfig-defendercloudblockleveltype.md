---
title: defenderCloudBlockLevelType 枚举类型
description: 云阻止级别的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: edc8f58be9c9bfdce904988503b42e20ed2d0bfb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755887"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

云阻止级别的可能值

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|默认值，使用默认Windows Defender 防病毒阻止级别并提供强检测，而不会增加检测合法文件的风险|
|high|1|High 应用强级别的检测。|
|highPlus|2|High + 使用高级别，并应用其他保护措施|
|zeroTolerance|3|零容限阻止所有未知可执行文件|




