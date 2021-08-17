---
title: managedAppDataEncryptionType 枚举类型
description: 表示对托管应用加密的应用数据的级别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d36cabacda74f33a5057257b5890f9496a9f64e28d2e36e808bbac8c17d9c24d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54145227"
---
# <a name="managedappdataencryptiontype-enum-type"></a>managedAppDataEncryptionType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示对托管应用加密的应用数据的级别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|useDeviceSettings|0|应用数据根据设备的默认设置进行加密。|
|afterDeviceRestart|1 |应用数据在设备重启时加密。|
|whenDeviceLockedExceptOpenFiles|2 |与此策略关联的应用数据在设备锁定时加密，打开的文件的数据除外|
|whenDeviceLocked|3 |与此策略关联的应用数据在设备锁定时加密|




