---
title: deviceDetail 资源类型
description: 指示与用于登录的设备相关联的设备详细信息。 包括设备浏览器和操作系统信息（如果设备是 Azure AD 托管）等信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 59d0912aefb5578be2bc1c65aeecd0897a94f899
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507245"
---
# <a name="devicedetail-resource-type"></a>deviceDetail 资源类型

命名空间： microsoft. graph 指示与用于登录的设备相关联的设备详细信息。 包括设备浏览器和操作系统信息（如果设备是 Azure AD 托管）等信息。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|浏览器|String|指示用于登录的浏览器信息。|
|deviceId|String|指用于登录的设备的 UniqueID。|
|displayName|String|指用于登录的设备的名称。|
|isCompliant|布尔|指示设备是否合规。|
|isManaged|Boolean|指示设备是否为托管设备。|
|operatingSystem|String|指示用于登录的 OS 名称和版本。|
|trustType|String|指示有关登录设备是否已加入工作区、AzureAD 加入和加入域的信息。 |

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
