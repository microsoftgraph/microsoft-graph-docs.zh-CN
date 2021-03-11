---
title: accessPackageResourceRoleScope 资源类型
description: 访问包资源角色作用域是一个对资源中的作用域和该资源中角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 8fa3e0a20646f2acf72d26d31c20bac674e751cd
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50720947"
---
# <a name="accesspackageresourcerolescope-resource-type"></a>accessPackageResourceRoleScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源角色作用域是一个对资源中的作用域的引用，也是该资源中该范围的角色的引用。  访问包将具有其目录中与该访问包相关的资源的访问包资源角色作用域。  当主题收到访问包分配时，主题将在每个访问包资源角色作用域的该范围内使用角色进行预配。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) | [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 集合 | 检索访问包 **的 accessPackageResourceRoleScope** 对象列表。 |
| [创建 accessPackageResourceRoleScope](../api/accesspackage-post-accesspackageresourcerolescopes.md) | | 为访问包 **创建新的 accessPackageResourceRoleScope** 对象。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdBy|String|只读。|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|id|String| 只读。|
|modifiedBy|String|只读。|
|modifiedDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResourceRole|[accessPackageResourceRole](accesspackageresourcerole.md)| 只读。 可为 NULL。|
|accessPackageResourceScope|[accessPackageResourceScope](accesspackageresourcescope.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRoleScope",
  "keyProperty": "id"
}-->

```json
{
   "createdBy":"String",
   "createdDateTime":"String (timestamp)",
   "id":"String (identifier)",
   "modifiedBy":"String",
   "modifiedDateTime":"String (timestamp)",
   "accessPackageResourceRole":{
      "id":"String (identifier)",
      "displayName":"String",
      "originSystem":"String",
      "originId":"String"
   },
   "accessPackageResourceScope":{
      "id":"String (identifier)",
      "displayName":"String",
      "description":"String",
      "originId":"String (identifier)",
      "originSystem":"String"
   }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRoleScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


