---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示可在应用程序之间共享设备的剪贴板的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7daab906ab376aea8b7540b88c6922a37ec23bd2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48684643"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示可在应用程序之间共享设备的剪贴板的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|允许在所有应用程序之间进行共享（托管或不允许）|
|managedAppsWithPasteIn|1|允许在启用了粘贴的所有托管应用之间进行共享|
|managedApps|双面|允许在所有托管应用之间进行共享|
|堵塞|第三章|已禁用应用程序之间的共享|





