---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作传递状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cda8bbb7f52898ddd042b8cba88b204907bfe9edff006510a61b6b36c7db66eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54239411"
---
# <a name="configurationmanageractiondeliverystatus-enum-type"></a>configurationManagerActionDeliveryStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Configuration Manager 设备操作传递状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|挂起以将操作传递至 ConfigurationManager|
|pendingDelivery|1 |挂起以将操作传递至 ConfigurationManager|
|deliveredToConnectorService|2 |操作将发送到 ConfigurationManager 连接器服务 (云) |
|failedToDeliverToConnectorService|3 |未能将操作发送到 ConfigurationManager 连接器服务 (云) |
|deliveredToOnPremisesServer|4 |操作将传递到 ConfigurationManager on-prem 服务器|




