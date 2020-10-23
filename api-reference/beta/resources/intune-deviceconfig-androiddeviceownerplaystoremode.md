---
title: androidDeviceOwnerPlayStoreMode 枚举类型
description: Android 设备所有者播放存储模式类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0c02c8f097c6f94df87203a7fee9d9a4abab8551
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707841"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a>androidDeviceOwnerPlayStoreMode 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者播放存储模式类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|allowList|1|只有策略中的应用程序可用，并且不在该策略中的任何应用程序将自动从设备中卸载。|
|阻止列表|双面|所有应用均可用，并且任何不应在设备上的应用程序应在应用程序策略中显式标记为 "已阻止"。|





