---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示设备剪贴板可以在应用之间共享的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b55b58cc0a5c3a514d805e149ace79c3e30f0a89
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60457377"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设备剪贴板可以在应用之间共享的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|是否允许在所有应用之间共享（托管或不共享）|
|managedAppsWithPasteIn|1|允许所有已启用粘贴的托管应用之间共享|
|managedApps|2|允许在所有托管应用之间共享|
|blocked|3|禁用应用之间的共享|



