---
title: androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型
description: Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
ms.openlocfilehash: 0287a26b4974bc0b376341ca91791d1fa768a9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041481"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a>androidDeviceOwnerAppAutoUpdatePolicyType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 设备所有者可能值的状态的设备的应用程序自动更新策略。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置;此值将被忽略。|
|userChoice|1|用户可以控制自动更新。|
|从不|2|应用程序永远不会自动更新。|
|wiFiOnly|3|应用程序仅自动更新通过 Wi-fi。|
|始终|4|应用程序在任何时候都自动更新。 可能话费数据。|





