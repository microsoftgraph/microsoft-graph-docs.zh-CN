---
title: vpnProviderType 枚举类型
description: 每个应用程序 VPN 的提供程序类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ea3e3fcac5fc84270fcdb63b6ab673cb9f55aea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27861283"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

每个应用程序 VPN 的提供程序类型。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|不明确地配置隧道通信。|
|appProxy|1|在应用层的隧道流量。|
|packetTunnel|2|在 IP 层的隧道流量。|





