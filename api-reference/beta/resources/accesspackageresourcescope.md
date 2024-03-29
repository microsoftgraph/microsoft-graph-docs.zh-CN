---
title: accessPackageResourceScope 资源类型
description: 在Azure AD中，访问包资源范围是一个对资源内范围的引用。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f403f6b2d7c88d1e24c579578c2c1b872bbbecdf
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651230"
---
# <a name="accesspackageresourcescope-resource-type"></a>accessPackageResourceScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[Azure AD中](entitlementmanagement-overview.md)，访问包资源范围是资源中具有多个范围的资源的作用域的引用。

通过使用列表 [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) 返回 [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 对象的集合，可以确定访问包资源作用域（对于已将角色添加到访问包的资源）。

如果资源位于访问包目录中，但尚未将其角色添加到访问包中，则可以通过使用[列表 accessPackageResources](../api/accesspackagecatalog-list-accesspackageresources.md)来确定访问包资源范围，并包括查询中。 `$expand=accessPackageResourceScopes,accessPackageResourceEnvironment`

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|范围的说明。|
|displayName|String|作用域显示名称。|
|id|String| 只读。|
|isRootScope|Boolean|如此 如果按层次结构排列范围，并且这是资源的顶部或根范围。|
|originId|String|资源中范围的唯一标识符，如源系统中定义。|
|originSystem|String|作用域的源系统。|
|roleOriginId|String|角色的源系统（如果不同）。|
|url|String|范围的资源定位器。|

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


