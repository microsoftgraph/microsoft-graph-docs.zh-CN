---
title: directoryRoleTemplate 资源类型
description: '表示目录角色模板。 目录角色模板指定目录角色 (directoryRole) 的属性值。 每个可在租户中激活的目录角色都有一个关联的目录角色模板对象。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下，仅激活公司管理员目录角色。 若要激活其他可用目录角色, 请将 POST 请求发送`/directoryRoles`到具有目录角色的 ID 的终结点, 该目录角色基于该角色模板的**roleTemplateId**参数在请求中的指定。 成功完成此请求后, 即可开始读取和分配目录角色的成员。 **注意**: 为 Users 目录角色公开了一个目录角色模板。 Users 目录角色是隐式的, 对目录客户端不可见。 租户中的每个用户都通过基础结构分配到此角色。 角色已激活。 请勿使用此模板。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5480e32498b4503cf4119b56c1025979c383a21c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029447"
---
# <a name="directoryroletemplate-resource-type"></a>directoryRoleTemplate 资源类型

表示目录角色模板。目录角色模板指定目录角色 ([directoryRole](directoryrole.md)) 的属性值。租户中每个已激活的目录角色都有一个相关的目录角色模板对象。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，仅激活公司管理员目录角色。要激活其他可用目录角色，发送 POST 请求到此目录角色模板 ID 的 `/directoryRoles` 端点，角色基于此模板，且此模板在请求的 **roleTemplateId** 参数中指定。在成功完成请求后，你可以开始读取，并将成员分配给目录角色。**注意**：目录角色模板针对用户目录角色公开。用户目录角色是隐式的，对目录客户端不可见。租户中的每个用户按基础结构分配到此角色。已激活该角色。请勿使用此模板。


## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 directoryRoleTemplate](../api/directoryroletemplate-get.md) | [directoryRoleTemplate](directoryroletemplate.md) |读取 directoryroletemplate 对象的属性和关系。|
|[列出 directoryRoleTemplate](../api/directoryroletemplate-list.md) | [directoryRoleTemplate](directoryroletemplate.md) 集合 |检索 directoryRoleTemplate 对象的列表。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|说明|String|可设置目录角色说明。只读。|
|displayName|String|可设置目录角色显示名称。只读。 |
|id|字符串|模板的的唯一标识符。继承自 [directoryObject](directoryobject.md)。在 POST 请求中指定 **roleTemplateId** 属性的目录角色模板的 **id** 将在租户中激活 [directoryRole](directoryrole.md)。密钥，不可为 NULL。只读。|

## <a name="relationships"></a>关系
无



## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.directoryRoleTemplate",
  "@odata.annotations": [
    {
      "capabilities": {
        "toppable": false
      }
    }
  ]
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryRoleTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
