---
title: vpnProviderType 枚举类型
description: 每个应用 VPN 的提供程序类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 180cd0ad739f67520e16945cf2e135a5c9ad88c4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819715"
---
# <a name="vpnprovidertype-enum-type"></a>vpnProviderType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

每个应用 VPN 的提供程序类型。

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|notConfigured|0|Tunnel未显式配置流量。|
|appProxy|1|Tunnel层的流量。|
|packetTunnel|2|Tunnel IP 层的流量。|



