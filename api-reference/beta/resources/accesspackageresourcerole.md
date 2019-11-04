---
title: accessPackageResourceRole 资源类型
description: 对资源中定义的角色的引用。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8b5ae5d321ac5fec86801ca11f60ead8a276fd73
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938917"
---
# <a name="accesspackageresourcerole-resource-type"></a>accessPackageResourceRole 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包资源角色是对在资源中定义的角色的引用，可在 access 程序包中使用。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|说明|String|资源角色的说明。|
|displayName|String|资源角色的显示名称，例如应用程序定义的角色。|
|id|字符串| 只读。|
|originId|字符串|源系统中资源角色的唯一标识符。 |
|originSystem|字符串|源系统中资源的类型。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 描述 |
|:-------------|:------------|:------------|
|accessPackageResource|[accessPackageResource](accesspackageresource.md)| 只读。可为空。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageResourceRole",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "originId": "String",
  "originSystem": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageResourceRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
