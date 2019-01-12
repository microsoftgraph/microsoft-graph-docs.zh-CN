---
title: deviceDetail 资源类型
description: 指示与用于登录的设备的设备详细信息。 如果设备是托管的 Azure AD，包括设备的浏览器和操作系统信息等信息。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971359"
---
# <a name="devicedetail-resource-type"></a>deviceDetail 资源类型
指示与用于登录的设备的设备详细信息。 如果设备是托管的 Azure AD，包括设备的浏览器和操作系统信息等信息。



## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|浏览器|字符串|指示使用的浏览器信息签名项。|
|deviceId|String|指用于签名中的设备的 UniqueID。|
|displayName|字符串|指用于签名中的设备的名称。|
|isCompliant|Boolean|指示是否符合设备。|
|isManaged|Boolean|指示托管设备。|
|operatingSystem|String|指示 OS 名称和用于签名中的版本。|
|trustType|String|指示是否已登录的设备上工作场所加入，AzureAD 加入，加入域的信息。 |

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
