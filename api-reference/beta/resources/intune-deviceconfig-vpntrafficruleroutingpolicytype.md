---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定对于 VPN 通信规则路由的策略。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 028e49085e4a1fa5f01ac59ff00fbafd8846dfb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415003"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>vpnTrafficRuleRoutingPolicyType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定对于 VPN 通信规则路由的策略。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未指定的路由策略。|
|splitTunnel|1|指定的应用程序的网络流量将通过 VPN 进行路由。|
|forceTunnel|2|所有网络流量将通过 VPN 进行都路由。|




