---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序需要应用程序角色。 RequiredResourceAccess 类型的**resourceAccess**属性是**ResourceAccess**的集合。
ms.openlocfilehash: 56e9b2b006d63d2a9abebc9e9585744b08438800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046865"
---
# <a name="resourceaccess-resource-type"></a>resourceAccess 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

指定 OAuth 2.0 权限范围或应用程序需要应用程序角色。 [RequiredResourceAccess](requiredresourceaccess.md)类型的**resourceAccess**属性是**ResourceAccess**的集合。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ID|Guid|一个资源应用程序公开[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)实例的唯一标识符。|
|type|字符串|指定的**id**属性引用[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)。 可能的值为"作用域"或"角色"。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
