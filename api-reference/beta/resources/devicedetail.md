---
title: deviceDetail 资源类型
description: 指示与用于登录的设备关联的设备详细信息。
localization_priority: Normal
author: spunukol
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3fb6b338793b77e3079922cd8c372e402488a22c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761126"
---
# <a name="devicedetail-resource-type"></a>deviceDetail 资源类型

命名空间：microsoft.graph 指示与用于登录的设备关联的设备详细信息。 包括设备浏览器和操作系统信息（如果设备是 Azure AD 托管设备）的信息。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|浏览器|String|指示用于登录的浏览器信息。|
|deviceId|String|引用用于登录的设备的唯一 ID。|
|displayName|String|指用于登录的设备的名称。|
|isCompliant|Boolean|指示设备是否符合要求。|
|isManaged|Boolean|指示设备是否受管理。|
|operatingSystem|String|指示用于登录的操作系统名称和版本。|
|trustType|String|指示已登录设备是否已加入 Workplace、AzureAD Joined、Domain Joined 的信息。 |

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


