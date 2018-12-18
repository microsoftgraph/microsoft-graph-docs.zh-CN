---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: tfitzmac
ms.openlocfilehash: 9f3d63b7e58b6f9c5ba369c3ceb12d06704c4725
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304555"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 枚举类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

FirewallPacketQueueingMethod 的可能值
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|deviceDefault|0|配置通过 Intune，没有值不会替代的用户配置设备默认值|
|禁用|1|停用数据包的队列|
|queueInbound|2|队列加密的入站的数据包|
|queueOutbound|3|用于呼叫转移队列解密出站数据包|
|queueBoth|4|队列入站和出站数据包|



