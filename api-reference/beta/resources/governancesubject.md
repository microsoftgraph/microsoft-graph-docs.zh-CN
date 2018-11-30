---
title: governanceSubject 资源类型
description: 表示用户、 组和管理特权标识管理 (PIM) 中的服务主体。
ms.openlocfilehash: c2129a0da488d4e7f425d6ef3596a955269e0da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042101"
---
# <a name="governancesubject-resource-type"></a>governanceSubject 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示用户、 组和管理特权标识管理 (PIM) 中的服务主体。


## <a name="properties"></a>属性
| 属性  | 类型       |说明|
|:----------|:----------|:----------|
|id         |字符串     | 主题的 id。|
|type       |字符串     |主题类型。 值可以是``User``， ``Group``，和``ServicePrincipal``。|
|displayName|字符串     |主题的显示名称。|
|email      |字符串     |用户使用者的电子邮件地址。 如果主题位于其他类型，它为空。|
|principalName|String   |主体的用户主体名称。 如果主题位于其他类型，它为空。|

## <a name="relationships"></a>Relationships
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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->