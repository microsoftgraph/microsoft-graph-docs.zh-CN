---
title: deviceManagementExchangeConnectorSyncType 枚举类型
description: Exchange 连接器同步请求的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2a78bf79990eb16ae6dbc62d4c324b905a79a7f2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405623"
---
# <a name="devicemanagementexchangeconnectorsynctype-enum-type"></a>deviceManagementExchangeConnectorSyncType 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Exchange 连接器同步请求的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|fullSync|0|在 Exchange 中发现的所有设备。|
|deltaSync|1|发现其增量同步窗口期间已更新的 Exchange 中的设备。|




