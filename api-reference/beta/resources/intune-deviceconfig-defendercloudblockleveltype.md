---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 928a39e25a02286159ba886bed9c1415b038edbf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001787"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

云块级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值是, 使用默认的 Windows Defender 防病毒阻止级别, 并提供强大的检测功能, 而不会增加检测合法文件的风险|
|高效|1|High 适用于强级别的检测。|
|highPlus|双面|高级别 + 使用高级别, 并应用附加保护措施|
|zeroTolerance|第三章|零耐受性阻止所有未知可执行文件|





