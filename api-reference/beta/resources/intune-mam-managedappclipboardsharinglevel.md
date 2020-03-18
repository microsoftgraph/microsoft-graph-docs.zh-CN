---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5f6153eeb4b76af9d8974b715b7c6342c646ba6e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782242"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示可在应用程序之间共享设备的剪贴板的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|允许在所有应用程序之间进行共享（托管或不允许）|
|managedAppsWithPasteIn|1|允许在启用了粘贴的所有托管应用之间进行共享|
|managedApps|双面|允许在所有托管应用之间进行共享|
|堵塞|第三章|已禁用应用程序之间的共享|



