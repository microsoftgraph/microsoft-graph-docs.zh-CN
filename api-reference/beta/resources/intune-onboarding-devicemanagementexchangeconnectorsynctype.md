---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47021a0a071995261f218cd4080026ababa33e0f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166596"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a>deviceManagementExchangeConnectorSyncType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

请求的 Exchange Connector 同步的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|完全同步|0|发现 Exchange 中的所有设备。|
|deltaSync|1|仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。|




