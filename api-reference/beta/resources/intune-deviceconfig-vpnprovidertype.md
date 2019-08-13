---
title: vpnProviderType 枚举类型
description: 每应用 VPN 的提供程序类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2ea4dee71a18a6ddca4519d8b421d2097fc7907b
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367643"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每应用 VPN 的提供程序类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|未显式配置隧道通信。|
|appProxy|1|应用程序层的隧道流量。|
|packetTunnel|双面|IP 层的隧道流量。|



