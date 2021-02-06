---
title: governanceSubject 资源类型
description: 表示在 PRIVILEGEd Identity Management 中管理的用户、组和服务主体 (PIM) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: eedcaff8538d5a0efa110b34cd6a72aef2a3210a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132671"
---
# <a name="governancesubject-resource-type"></a>governanceSubject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示在 PRIVILEGEd Identity Management 中管理的用户、组和服务主体 (PIM) 。


## <a name="properties"></a>属性
| 属性  | 类型       |说明|
|:----------|:----------|:----------|
|id         |字符串     | 主题的 ID。|
|type       |字符串     |主题的类型。 值可以是 ``User`` 、 ``Group`` 和 ``ServicePrincipal`` 。|
|displayName|字符串     |主题显示名称。|
|email      |字符串     |用户主题的电子邮件地址。 如果主题为其他类型的主题，则为空。|
|principalName|String   |用户主题的主体名称。 如果主题为其他类型的主题，则为空。|

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


