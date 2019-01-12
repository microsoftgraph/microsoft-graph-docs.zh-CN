---
title: androidDeviceOwnerSystemUpdateInstallType 枚举类型
description: Android 设备所有者的系统更新类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9a46d60972bab46fa0e2cda8d03a090bd8b810a9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980970"
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





