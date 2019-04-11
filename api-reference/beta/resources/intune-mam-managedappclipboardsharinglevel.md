---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d18d09f2ba37b8b062f3d19ae5cf971d886f278
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777590"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示可在应用程序之间共享设备的剪贴板的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|允许在所有应用程序之间进行共享 (托管或不允许)|
|managedAppsWithPasteIn|1|允许在启用了粘贴的所有托管应用之间进行共享|
|managedApps|双面|允许在所有托管应用之间进行共享|
|堵塞|第三章|已禁用应用程序之间的共享|





