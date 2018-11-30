---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: Android 设备所有者的系统更新类型。
ms.openlocfilehash: e9f23fd96ed0965b6693776858082e2df4925f37
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045418"
---
# <a name="androiddeviceownersystemupdateinstalltype-enum-type"></a>androidDeviceOwnerSystemUpdateInstallType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Android 设备所有者的系统更新类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|设备默认行为，通常会提示用户接受系统更新。|
|延迟|1|为 30 天推迟自动安装更新。|
|窗口|2|在日常维护时段内自动安装。|
|automatic|3|自动尽快安装更新。|





