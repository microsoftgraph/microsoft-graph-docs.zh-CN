---
title: deviceExchangeAccessStateSummary 资源类型
description: 设备 Exchange 访问状态摘要
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7309bfa0d4714453a0477d2ec9948650b0d7f6ba
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2021
ms.locfileid: "60453840"
---
# <a name="deviceexchangeaccessstatesummary-resource-type"></a>deviceExchangeAccessStateSummary 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

设备 Exchange 访问状态摘要

## <a name="properties"></a>属性
|属性|类型|说明|
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



