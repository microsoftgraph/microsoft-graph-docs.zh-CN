---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定到特定 Windows 隐私数据类别的访问级别。
ms.openlocfilehash: 09db03706795cc2aba4cc0c93dce87dc7069cd3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049239"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

确定到特定 Windows 隐私数据类别的访问级别。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|指定无访问级别，没有方法。 设备可能表现，可以如 UserInControl 或 ForceAllow 中所示。 它可能依赖的隐私数据已访问它们，Windows 版本和其他因素。|
|forceAllow|1|应用程序将可以访问指定的隐私数据。|
|forceDeny|2|应用程序将被拒绝访问指定的隐私数据。|
|userInControl|3|应用程序尝试访问指定的隐私数据时，将会提示用户。|





