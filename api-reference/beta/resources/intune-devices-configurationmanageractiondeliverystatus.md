---
title: configurationManagerActionDeliveryStatus 枚举类型
description: Configuration Manager 设备操作传递状态
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e776d03e4d785191ff3463bae125d786250ee22d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59111003"
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
|pendingDelivery|1|挂起以将操作传递至 ConfigurationManager|
|deliveredToConnectorService|2|操作将发送到 ConfigurationManager 连接器服务 (云) |
|failedToDeliverToConnectorService|3|未能将操作发送到 ConfigurationManager 连接器服务 (云) |
|deliveredToOnPremisesServer|4 |操作将传递到 ConfigurationManager on-prem 服务器|



