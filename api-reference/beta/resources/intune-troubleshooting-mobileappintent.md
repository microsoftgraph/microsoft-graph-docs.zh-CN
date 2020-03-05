---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a530c7b67d4bde5829f11471434341d365d3275
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523343"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备上的移动应用的状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|可用|0|可用|
|notAvailable|1 |不可用|
|requiredInstall|2 |必需的安装|
|requiredUninstall|3 |必需的卸载|
|requiredAndAvailableInstall|4 |RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5 |AvailableInstallWithoutEnrollment|
|排除|6 |排除|



