---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定 VPN 流量规则的路由策略。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5782555214897ec0513ab7293adf1d877ec5f96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042420"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>vpnTrafficRuleRoutingPolicyType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定 VPN 流量规则的路由策略。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未指定路由策略。|
|splitTunnel|1 |将通过 VPN 路由指定应用的网络流量。|
|forceTunnel|2 |所有网络流量将通过 VPN 路由。|






