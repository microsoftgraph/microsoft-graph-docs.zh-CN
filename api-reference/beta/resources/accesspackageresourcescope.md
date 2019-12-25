---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权限管理中，访问包资源作用域是对资源中的范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1418e2cb21a1023e864d842b760006e05f3afb03
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870962"
---
# <a name="accesspackageresourcescope-resource-type"></a>accessPackageResourceScope 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源作用域是对包含多个作用域的资源中的范围的引用。

您可以通过使用[List accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md)返回[accessPackageResourceRoleScope](accesspackageresourcerolescope.md)对象的集合，来确定已添加到 access 程序包的资源的访问包资源范围。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|作用域的说明。|
|displayName|字符串|作用域的显示名称。|
|id|字符串| 只读。|
|isRootScope|Boolean|如此如果作用域在层次结构中排列，这是资源的顶部或根作用域。|
|originId|String|在源系统中定义的资源中的范围的唯一标识符。|
|originSystem|String|作用域的源系统。|
|roleOriginId|String|角色的原始系统（如果不同）。|
|url|String|作用域的资源定位器。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceScope",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "isRootScope": true,
  "originId": "String",
  "originSystem": "String",
  "roleOriginId": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
