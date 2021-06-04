---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ee3f6ddb47025dfc4ff29305f45538cf23bfa8c6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754586"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>deviceExchangeAccessStateSummary 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备 Exchange 访问状态摘要

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|allowedDeviceCount|Int32|Exchange 访问状态为允许的设备总数。|
|blockedDeviceCount|Int32|Exchange 访问状态为阻止的设备总数。|
|quarantinedDeviceCount|Int32|Exchange 访问状态为隔离的设备总数。|
|unknownDeviceCount|Int32|Exchange 访问状态为未知的设备总数。|
|unavailableDeviceCount|Int32|无法找到其 Exchange 访问状态的设备总数。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": 1024,
  "blockedDeviceCount": 1024,
  "quarantinedDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "unavailableDeviceCount": 1024
}
```




