---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: 适用于 Android 设备所有者的系统更新类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6f99ba32a5461913579a23e7fe8f29a3c0b6950
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163656"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a>androidDeviceOwnerSystemUpdateInstallType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

适用于 Android 设备所有者的系统更新类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认行为, 通常提示用户接受系统更新。|
|推迟|1|将更新自动安装推迟30天。|
|开|双面|在每日维护时段内自动安装。|
|自动|第三章|尽快自动安装更新。|




