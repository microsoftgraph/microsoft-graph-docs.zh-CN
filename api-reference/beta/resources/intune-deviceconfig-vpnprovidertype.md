---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e47f4d20cb843b62928c6c66e468d00f5a4f743
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561913"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每应用 VPN 的提供程序类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未显式配置隧道通信。|
|appProxy|1|应用程序层的隧道流量。|
|packetTunnel|2 |IP 层的隧道流量。|





