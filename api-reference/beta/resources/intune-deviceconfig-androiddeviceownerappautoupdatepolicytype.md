---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
localization_priority: Normal
ms.openlocfilehash: 721d08220553bf6acfaac0f84bf0d71725c39ba6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834116"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|未配置;此值将被忽略。|
|userChoice|1|用户可以控制自动更新。|
|从不|2|应用程序永远不会自动更新。|
|wiFiOnly|3|应用程序仅自动更新通过 Wi-fi。|
|始终|4|应用程序在任何时候都自动更新。 可能话费数据。|





