---
title: managedAppClipboardSharingLevel 枚举类型
description: 代表到设备的剪贴板可能共享应用程序之间的级别
ms.openlocfilehash: 71c4ab2d629fdfee3ded68612d7060a0fa069809
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048942"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表到设备的剪贴板可能共享应用程序之间的级别
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|共享之间所有的应用程序、 托管或不允许|
|managedAppsWithPasteIn|1|共享之间不允许与粘贴中的所有托管应用程序启用|
|managedApps|2|共享之间所有的托管应用程序不允许|
|已阻止|3|禁用应用程序之间共享|





