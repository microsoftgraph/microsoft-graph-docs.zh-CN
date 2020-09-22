---
title: mobileAppIntent 枚举类型
description: 指示设备上的移动应用的状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f6da589015b5120add046eabfa146069cc349951
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075761"
---
# <a name="mobileappintent-enum-type"></a>mobileAppIntent 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示设备上的移动应用的状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|可用|0|可用|
|notAvailable|1 |不可用|
|requiredInstall|2 |必需的安装|
|requiredUninstall|第三章|必需的卸载|
|requiredAndAvailableInstall|4 |RequiredAndAvailableInstall|
|availableInstallWithoutEnrollment|5 |AvailableInstallWithoutEnrollment|
|排除|6 |排除|






