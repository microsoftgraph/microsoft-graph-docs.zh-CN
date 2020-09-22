---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 12223e48d60fffbfa0ad3b222b490c3e59295094
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029615"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a>deviceManagementExchangeConnectorSyncType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

请求的 Exchange Connector 同步的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|完全同步|0|发现 Exchange 中的所有设备。|
|deltaSync|1 |仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。|






