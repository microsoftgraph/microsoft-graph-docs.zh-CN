---
title: vpnServiceExceptionAction 枚举类型
description: 对特定服务要采取 VPN 操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: baf1fa3bf6edcb3358c8ae56d2572365702c41273a04bd578c2c98af5e68d0ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139598"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>vpnServiceExceptionAction 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

对特定服务要采取 VPN 操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|forceTrafficViaVPN|0|使该服务的所有流量都通过 VPN|
|allowTrafficOutside|1 |允许 VPN 外部的服务|
|dropTraffic|2 |从服务删除所有流量|




