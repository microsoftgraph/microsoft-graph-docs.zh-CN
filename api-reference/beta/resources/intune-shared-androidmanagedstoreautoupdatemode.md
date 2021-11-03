---
title: androidManagedStoreAutoUpdateMode 枚举类型
description: 在分配时设置的 Android 托管应用商店应用的自动更新优先顺序。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: adaca71257f5ee18cec8af62bfaf1e12d201ba3f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60695527"
---
# <a name="androidmanagedstoreautoupdatemode-enum-type"></a>androidManagedStoreAutoUpdateMode 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

在分配时设置的 Android 托管应用商店应用的自动更新优先顺序。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|default|0|设备的默认 (行为必须连接到 Wifi、充电且未主动) 。|
|延迟|1|更新在应用过期后最多延迟 90 天。|
|priority|2|应用由开发人员尽快更新。 如果设备联机，它将在数分钟内更新。|
|unknownFutureValue|3|未知未来模式 (保留，当前未) 。|



