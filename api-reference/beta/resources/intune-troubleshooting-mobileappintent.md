---
title: mobileAppIntent 枚举类型
description: 指示在设备上的移动应用程序的状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b8119cd188823beabf5b273e5324d0098e5b9ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875409"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

指示在设备上的移动应用程序的状态。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|可用|0|可用|
|notAvailable|1|不可用|
|requiredInstall|2|所需的安装|
|requiredUninstall|3|需要的卸载|
|requiredAndAvailableInstall|4|RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5|AvailableInstallWithoutEnrollment|
|排除|6|排除|





