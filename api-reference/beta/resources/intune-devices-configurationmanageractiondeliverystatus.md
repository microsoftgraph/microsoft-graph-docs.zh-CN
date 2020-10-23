---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09c7b1be3a5fdfc33a064d2a9208daa68ba4263e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733984"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>configurationManagerActionDeliveryStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Configuration Manager 设备操作的传递状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|挂起，将操作传递给 ConfigurationManager|
|pendingDelivery|1|挂起，将操作传递给 ConfigurationManager|
|deliveredToConnectorService|双面|将操作发送到 ConfigurationManager Connector service (云) |
|failedToDeliverToConnectorService|第三章|无法将操作发送到 ConfigurationManager Connector service (云) |
|deliveredToOnPremisesServer|4 |操作传递给 ConfigurationManager on-本地 server|





