---
title: zebraFotaNetworkType 枚举类型
description: 表示 Zebra FOTA 部署的各种网络类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9026673271e63ab386ad7a2c16a9fbc276ea52ba
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213180"
---
# <a name="zebrafotanetworktype-enum-type"></a>zebraFotaNetworkType 枚举类型

命名空间：microsoft.graph

> **重要：**/beta 版本下的 Microsoft Graph API 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 Zebra FOTA 部署的各种网络类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|任意|0|无论当前网络类型如何，设备都将安装更新。|
|无线|1|只有在连接到 WiFi 网络时，设备才会安装更新。|
|细胞|2|仅当连接到手机网络时，设备才会安装更新。|
|wifiAndCellular|3|连接 WiFi 和 Cellular 时，设备将安装更新。|
|unknownFutureValue|99|未知的未来枚举值。|




