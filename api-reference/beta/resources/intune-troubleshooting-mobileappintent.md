---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7aa8da2d0cb32f641a050ae565568991b1b42ef4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42765081"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备上的移动应用的状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|可用|0|可用|
|notAvailable|1|不可用|
|requiredInstall|双面|必需的安装|
|requiredUninstall|第三章|必需的卸载|
|requiredAndAvailableInstall|4 |RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5 |AvailableInstallWithoutEnrollment|
|排除|6 |排除|



