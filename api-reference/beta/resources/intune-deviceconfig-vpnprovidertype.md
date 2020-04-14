---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2809f0297ba952d1c302bc0597ab3e00bb33ab95
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412036"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每应用 VPN 的提供程序类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未显式配置隧道通信。|
|appProxy|1|应用程序层的隧道流量。|
|packetTunnel|双面|IP 层的隧道流量。|



