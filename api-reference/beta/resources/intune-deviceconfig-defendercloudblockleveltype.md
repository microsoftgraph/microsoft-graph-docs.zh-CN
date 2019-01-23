---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425909"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

云块级别的可能值

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强检测而不会提高检测的风险合法文件|
|高|1|高适用检测强的级别。|
|highPlus|2|高 + 使用的高级别和应用添加保护措施|
|zeroTolerance|3|零公差阻止所有未知的可执行文件|




