---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472fd157ed26b8b446e272d37baa135584cbbe0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558251"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备上的移动应用的状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|可用|0|可用|
|notAvailable|1|不可用|
|requiredInstall|2 |必需的安装|
|requiredUninstall|3 |必需的卸载|
|requiredAndAvailableInstall|4 |RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5 |AvailableInstallWithoutEnrollment|
|排除|6 |排除|



