---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作的传递状态
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58dca2b1ecb5419a3f56889a55c0816f492af430
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785089"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>configurationManagerActionDeliveryStatus 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Configuration Manager 设备操作的传递状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|挂起，将操作传递给 ConfigurationManager|
|pendingDelivery|1|挂起，将操作传递给 ConfigurationManager|
|deliveredToConnectorService|双面|将操作发送到 ConfigurationManager 连接器服务（云）|
|failedToDeliverToConnectorService|第三章|无法将操作发送到 ConfigurationManager 连接器服务（云）|
|deliveredToOnPremisesServer|4 |操作传递给 ConfigurationManager on-本地 server|



