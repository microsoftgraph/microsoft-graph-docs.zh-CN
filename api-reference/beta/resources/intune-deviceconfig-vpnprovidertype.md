---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b064c86413d84a06884de9728ccfa9cb83d61d2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787346"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每应用 VPN 的提供程序类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未显式配置隧道通信。|
|appProxy|1|应用程序层的隧道流量。|
|packetTunnel|双面|IP 层的隧道流量。|



