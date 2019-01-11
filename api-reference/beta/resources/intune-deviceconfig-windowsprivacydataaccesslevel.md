---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定到特定 Windows 隐私数据类别的访问级别。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888772"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a>windowsPrivacyDataAccessLevel 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

确定到特定 Windows 隐私数据类别的访问级别。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|指定无访问级别，没有方法。 设备可能表现，可以如 UserInControl 或 ForceAllow 中所示。 它可能依赖的隐私数据已访问它们，Windows 版本和其他因素。|
|forceAllow|1|应用程序将可以访问指定的隐私数据。|
|forceDeny|2|应用程序将被拒绝访问指定的隐私数据。|
|userInControl|3|应用程序尝试访问指定的隐私数据时，将会提示用户。|





