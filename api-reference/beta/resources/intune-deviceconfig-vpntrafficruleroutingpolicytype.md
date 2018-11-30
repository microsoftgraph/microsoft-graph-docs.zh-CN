---
title: vpnTrafficRuleRoutingPolicyType 枚举类型
description: 指定对于 VPN 通信规则路由的策略。
ms.openlocfilehash: df51851ef0820f5982a6689421503364e9064c78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044236"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a>vpnTrafficRuleRoutingPolicyType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

指定对于 VPN 通信规则路由的策略。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|无|0|未指定的路由策略。|
|splitTunnel|1|指定的应用程序的网络流量将通过 VPN 进行路由。|
|forceTunnel|2|所有网络流量将通过 VPN 进行都路由。|





