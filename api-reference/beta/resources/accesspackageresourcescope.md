---
title: accessPackageResourceScope 资源类型
description: 在 Azure AD 权利管理中，访问包资源范围是资源内范围的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1491028bb566e8742dcfc1e4928681f61e5272c7
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133586"
---
# <a name="accesspackageresourcescope-resource-type"></a>accessPackageResourceScope 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利管理](entitlementmanagement-root.md)中，访问包资源范围是资源内对具有多个作用域的资源的作用域的引用。

通过使用列表 [accessPackageResourceRoleScopes](../api/accesspackage-list-accesspackageresourcerolescopes.md) 返回 [accessPackageResourceRoleScope](accesspackageresourcerolescope.md) 对象的集合，可以确定已添加到访问包的资源的访问包资源范围。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|字符串|范围的说明。|
|displayName|字符串|作用域显示名称的作用域。|
|id|字符串| 只读。|
|isRootScope|Boolean|如此 如果范围按层次结构排列，并且这是资源的顶部或根范围。|
|originId|字符串|资源中范围的唯一标识符，如源系统中定义。|
|originSystem|字符串|范围的源系统。|
|roleOriginId|字符串|角色的源系统（如果不同）。|
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


