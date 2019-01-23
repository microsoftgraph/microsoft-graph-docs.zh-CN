---
title: androidKeyguardFeature 枚举类型
description: Android keyguard 功能。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df89e1e9170bf2e3691116e27125514c7e0a6de9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429370"
---
# <a name="androidkeyguardfeature-enum-type"></a>androidKeyguardFeature 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Android keyguard 功能。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未配置;此值将被忽略。|
|摄像机|1|在安全 keyguard 屏幕上时的照相机用法。|
|通知|2|显示在安全 keyguard 屏幕上时的通知。|
|unredactedNotifications|3|在安全 keyguard 屏幕上时显示 unredacted 通知。|
|trustAgents|4|信任代理时安全 keyguard 屏幕上的状态。|
|指纹|5|指纹传感器使用率在安全 keyguard 屏幕上时。|
|remoteInput|6|在安全 keyguard 屏幕上时通知文本项。|
|allFeatures|7|在安全 keyguard 屏幕上时的所有 keyguard 功能。|




