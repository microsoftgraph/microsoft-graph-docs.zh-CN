---
title: firewallPacketQueueingMethodType 枚举类型
description: FirewallPacketQueueingMethod 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d9b4591ceff59becfa6f9fb17d490c56d59c9703
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833010"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

FirewallPacketQueueingMethod 的可能值
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|配置通过 Intune，没有值不会替代的用户配置设备默认值|
|禁用|1|停用数据包的队列|
|queueInbound|2|队列加密的入站的数据包|
|queueOutbound|3|用于呼叫转移队列解密出站数据包|
|queueBoth|4|队列入站和出站数据包|





