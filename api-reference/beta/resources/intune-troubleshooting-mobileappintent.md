---
title: mobileAppIntent 枚举类型
description: 指示在设备上的移动应用程序的状态。
author: tfitzmac
ms.openlocfilehash: 0a230279a947ab60314a53872670fff871eff745
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347227"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

指示在设备上的移动应用程序的状态。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|可用|0|可用|
|notAvailable|1|不可用|
|requiredInstall|2|所需的安装|
|requiredUninstall|3|需要的卸载|
|requiredAndAvailableInstall|4|RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5|AvailableInstallWithoutEnrollment|
|排除|6|排除|





