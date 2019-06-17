---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: 请求的 Exchange Connector 同步的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04cd9e55b03e21bd4e99c56144ea05cabd1ecd7b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993002"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a>deviceManagementExchangeConnectorSyncType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

请求的 Exchange Connector 同步的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|完全同步|0|发现 Exchange 中的所有设备。|
|deltaSync|1|仅发现 Exchange 中的设备在 "delta sync" 窗口中已更新。|





