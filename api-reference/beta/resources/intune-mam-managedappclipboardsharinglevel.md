---
title: managedAppClipboardSharingLevel 枚举类型
description: 表示设备剪贴板可以在应用之间共享的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8bf20224470da6d1040befc03ff5eb2ead3db0a0c96a4071ebea34111f922966
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54248388"
---
# <a name="managedappclipboardsharinglevel-enum-type"></a>managedAppClipboardSharingLevel 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示设备剪贴板可以在应用之间共享的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|allApps|0|是否允许在所有应用之间共享（托管或不共享）|
|managedAppsWithPasteIn|1 |允许所有已启用粘贴的托管应用之间共享|
|managedApps|2 |允许在所有托管应用之间共享|
|blocked|3 |禁用应用之间的共享|




