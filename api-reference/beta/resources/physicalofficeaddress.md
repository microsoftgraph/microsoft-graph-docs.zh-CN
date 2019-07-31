---
title: physicalOfficeAddress 资源类型
description: 表示某个资源 (如联系人或事件) 的业务地址。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8299f72032cfb7910583fcd4dbefe914f054648e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966095"
---
# <a name="physicalofficeaddress-resource-type"></a>physicalOfficeAddress 资源类型

表示资源 (如组织联系人) 的业务地址。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|city|String|城市。|
|countryOrRegion|字符串|国家或地区。它是任意格式的字符串值，例如“United States”。|
|officeLocation  | String | 组织联系人的办公地点, 如建筑物和办公室号码。  |
|postalCode|String|邮政编码。|
|state|String|省/市/自治区。|
|street|String|街道。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.physicalOfficeAddress"
}-->

```json
{
  "city": "string",
  "countryOrRegion": "string",
  "officeLocation": "string",
  "postalCode": "string",
  "state": "string",
  "street": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "physicalOfficeAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
