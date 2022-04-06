---
title: governanceSubject 资源类型
description: 表示在 PIM 管理中心中管理的用户、Privileged Identity Management () 。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: japere
ms.openlocfilehash: 99e668cc18ff38f8a4b26c11d514beddcc020e00
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509635"
---
# <a name="governancesubject-resource-type"></a>governanceSubject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 PIM 管理中心中管理的用户、Privileged Identity Management () 。


## <a name="properties"></a>属性
| 属性  | 类型       |说明|
|:----------|:----------|:----------|
|id         |字符串     | 主题的 ID。|
|type       |字符串     |主题的类型。 值可以是 、 ``User````Group``和 ``ServicePrincipal``。|
|displayName|String     |主题显示名称。|
|email      |String     |用户主题的电子邮件地址。 如果主题位于其他类型的中，则为空。|
|principalName|String   |用户主题的主体名称。 如果主题位于其他类型的中，则为空。|

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


