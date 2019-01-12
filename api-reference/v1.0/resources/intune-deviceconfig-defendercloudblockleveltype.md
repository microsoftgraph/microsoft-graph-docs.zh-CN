---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e27ec7042522d7d4c83463b062cdc0c4c109daeb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951409"
---
# <a name="defendercloudblockleveltype-enum-type"></a>defenderCloudBlockLevelType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

云块级别的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强检测而不会提高检测的风险合法文件|
|高|1|高适用检测强的级别。|
|highPlus|2|高 + 使用的高级别和应用添加保护措施|
|zeroTolerance|3|零公差阻止所有未知的可执行文件|



