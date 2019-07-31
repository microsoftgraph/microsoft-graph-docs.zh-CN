---
title: governanceSubject 资源类型
description: 表示在特权标识管理 (PIM) 中管理的用户、组和服务主体。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26f6c6904de97fc96eb1b29b9bcbc376bcf69c61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005973"
---
# <a name="governancesubject-resource-type"></a>governanceSubject 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在特权标识管理 (PIM) 中管理的用户、组和服务主体。


## <a name="properties"></a>属性
| 属性  | 类型       |说明|
|:----------|:----------|:----------|
|id         |String     | 主题的 id。|
|type       |字符串     |主题的类型。 值可以是``User``、 ``Group``和。 ``ServicePrincipal``|
|displayName|String     |主题的显示名称。|
|email      |String     |用户主题的电子邮件地址。 如果主题在其他类型中, 则为空。|
|principalName|String   |用户主题的主体名称。 如果主题在其他类型中, 则为空。|

## <a name="relationships"></a>关系
无


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
