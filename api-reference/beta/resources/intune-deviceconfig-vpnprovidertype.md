---
title: vpnProviderType 枚举类型
description: 每个应用 VPN 的提供程序类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: af9951628865c2a743a0f2b3ea04aafeac2438e76373f9b652e4921eab2708e0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54224773"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每个应用 VPN 的提供程序类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|notConfigured|0|Tunnel未显式配置流量。|
|appProxy|1 |Tunnel应用程序层的流量。|
|packetTunnel|2 |Tunnel IP 层的流量。|




