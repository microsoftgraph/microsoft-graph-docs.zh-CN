---
title: physicalOfficeAddress 资源类型
description: 表示资源（如联系人或事件）的业务地址。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: dkershaw10
ms.openlocfilehash: 55faeb615225aa7c3f3f3c9babf69ad8f9952fc8acdf2d5bf9f05b1a94edc236
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54187607"
---
# <a name="physicalofficeaddress-resource-type"></a>physicalOfficeAddress 资源类型

命名空间：microsoft.graph

表示资源（如组织联系人）的业务地址。

## <a name="properties"></a>属性

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|城市|String|城市。|
|countryOrRegion|String|国家或地区。它是任意格式的字符串值，例如“United States”。|
|officeLocation  | String | Office联系人的位置，例如建筑物和办公室号码。  |
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


