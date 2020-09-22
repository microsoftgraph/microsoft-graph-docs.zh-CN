---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。 其中包括设备浏览器和操作系统等信息，以及设备是否为 Azure AD 托管。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3a756df15be02544f843e6176677f26ea7e95678
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018701"
---
# <a name="devicedetail-resource-type"></a>deviceDetail 资源类型

命名空间：microsoft.graph

指示与用于登录的设备相关联的设备详细信息。 其中包括设备浏览器和操作系统等信息，以及设备是否为 Azure AD 托管。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|浏览器|String|指示用于登录的浏览器信息。|
|deviceId|String|指用于登录的设备的 UniqueID。|
|displayName|String|表示用于登录的设备的名称。|
|isCompliant|Boolean|指示设备是否合规。|
|isManaged|Boolean|指示设备是否为托管设备。|
|operatingSystem|String|指示用于登录的操作系统名称和版本。|
|trustType|String|提供有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

