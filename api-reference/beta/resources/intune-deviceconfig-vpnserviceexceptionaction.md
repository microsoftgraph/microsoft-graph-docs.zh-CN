---
title: vpnServiceExceptionAction 枚举类型
description: 要对特定服务执行的 VPN 操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1310d91da9a7ea8e3a6274acd48e8ebc1359cafd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636712"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>vpnServiceExceptionAction 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对特定服务执行的 VPN 操作。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|forceTrafficViaVPN|0|使来自该服务的所有流量都通过 VPN|
|allowTrafficOutside|1 |允许 VPN 外部的服务|
|dropTraffic|2 |从服务中删除所有流量|



