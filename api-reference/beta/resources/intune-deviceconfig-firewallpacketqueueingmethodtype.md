---
title: firewallPacketQueueingMethodType 枚举类型
description: firewallPacketQueueingMethod 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b496651cb8735a06afd5ae68e56e4078095180dc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817101"
---
# <a name="firewallpacketqueueingmethodtype-enum-type"></a>firewallPacketQueueingMethodType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

firewallPacketQueueingMethod 的可能值

## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|deviceDefault|0|Intune 未配置任何值，请勿替代用户配置的设备默认值|
|disabled|1|禁用数据包队列|
|queueInbound|2|将入站加密数据包排入队列|
|queueOutbound|3|队列解密的出站数据包用于转发|
|queueBoth|4 |对入站和出站数据包进行排队|



