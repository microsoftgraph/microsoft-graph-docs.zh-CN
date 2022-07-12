---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示设备剪贴板可在应用之间共享的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bef107cb05cbc654663033042e4d032b2c54475e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66722927"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设备剪贴板可在应用之间共享的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|允许在所有应用之间共享，无论是否托管|
|managedAppsWithPasteIn|1|允许在启用了粘贴的所有托管应用之间共享|
|managedApps|2|允许在所有托管应用之间共享|
|封锁|3|已禁用应用之间的共享|





