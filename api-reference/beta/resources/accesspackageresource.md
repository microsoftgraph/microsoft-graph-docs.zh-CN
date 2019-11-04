---
title: accessPackageResource 资源类型
description: 访问包资源是对与目录关联的资源的引用。可在一个或多个访问包中使用的角色。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e964a8ce2e9bd4165a29037a56ec4f95fe969422
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938924"
---
# <a name="accesspackageresource-resource-type"></a>accessPackageResource 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源是对与目录关联的资源的引用。可在一个或多个访问包中使用的角色。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [列出 accessPackageCatalog 资源](../api/accesspackagecatalog-list-accesspackageresources.md) | [accessPackageResource](accesspackageresource.md)集合 | 检索 accesspackageresource 对象的列表。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|addedBy|字符串|只读。|
|addedOn|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|description|String|资源的说明。|
|displayName|字符串|资源的显示名称，例如应用程序名称、组名称或网站名称。|
|id|字符串| 只读。|
|isPendingOnboarding|Boolean|如果资源尚不可用于工作分配，则为 True。|
|originId|字符串|源系统中资源的唯一标识符。 |
|originSystem|字符串|源系统中资源的类型。|
|resourceType|字符串|资源的类型，例如， `Application`如果是 Azure AD 连接的应用程序。|
|url|String|资源的唯一资源定位器，例如用于将用户签名到应用程序的 URL。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 描述 |
|:-------------|:------------|:------------|
|accessPackageResourceRoles|[accessPackageResourceRole](accesspackageresourcerole.md)集合| 只读。 可为 Null。|
|accessPackageResourceScopes|[accessPackageResourceScope](accesspackageresourcescope.md)集合| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResource",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "addedBy": "String",
  "addedOn": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isPendingOnboarding": true,
  "originId": "String",
  "originSystem": "String",
  "resourceType": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
