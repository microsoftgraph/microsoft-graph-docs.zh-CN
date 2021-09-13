---
title: androidDeviceOwnerPlayStoreMode 枚举类型
description: Android 设备所有者 Play Store 模式类型。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d7110a4dcc255e47866b3746273d6a87c670f12e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106572"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a>androidDeviceOwnerPlayStoreMode 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android 设备所有者 Play Store 模式类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置|
|allowList|1|只有策略中的应用可用，任何不在策略中的应用将自动从设备卸载。|
|blockList|2|所有应用都可用，不应在设备上的任何应用都应在应用程序策略中明确标记为"已阻止"。|



