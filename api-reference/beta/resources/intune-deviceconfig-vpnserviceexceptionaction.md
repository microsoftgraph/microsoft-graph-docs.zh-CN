---
title: vpnServiceExceptionAction 枚举类型
description: 要对特定服务执行的 VPN 操作。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 069b7dc910a7c4ce9e281235aefc52b498519351
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279435"
---
# <a name="vpnserviceexceptionaction-enum-type"></a>vpnServiceExceptionAction 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

要对特定服务执行的 VPN 操作。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|forceTrafficViaVPN|0|使来自该服务的所有流量都通过 VPN|
|allowTrafficOutside|1|允许 VPN 外部的服务|
|dropTraffic|双面|从服务中删除所有流量|




