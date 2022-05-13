---
title: governanceSubject 资源类型
description: 表示Privileged Identity Management (PIM) 中管理的用户、组和服务主体。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: f898c844a9bf2d461cf73e02abf1852e012c1825
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397570"
---
# <a name="governancesubject-resource-type"></a>governanceSubject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示Privileged Identity Management (PIM) 中管理的用户、组和服务主体。


## <a name="properties"></a>属性
| 属性  | 类型       |说明|
|:----------|:----------|:----------|
|id         |String     | 主题的 ID。|
|type       |String     |主题的类型。 值可以是 ``User``， ``Group``和 ``ServicePrincipal``.|
|displayName|字符串     |主题的显示名称。|
|email      |String     |用户主题的电子邮件地址。 如果主题在其他类型中，则为空。|
|principalName|String   |用户主体的主体名称。 如果主题在其他类型中，则为空。|

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


