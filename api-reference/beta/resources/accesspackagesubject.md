---
title: accessPackageSubject 资源类型
description: 在 Azure AD 权限管理中，访问包分配的主题。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0f71b23e48c818747a2b70b52ec8b4baa53bf118
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508490"
---
# <a name="accesspackagesubject-resource-type"></a>accessPackageSubject 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在[AZURE AD 权限管理](entitlementmanagement-root.md)中，访问包主题是可以配置为请求或分配访问包的用户、服务主体或其他实体。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|字符串|主题的显示名称。|
|email|String|主题的电子邮件地址。|
|id|String| 只读。|
|objectId|String|主题的对象 ID。|
|principalName|String|主题的主体名称（如果已知）。|
|type|字符串|主题的资源类型。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "Administrator",
  "email": "admin@contoso.com",
  "id": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
  "objectId": "cc754ed5-f598-45c0-aaf0-fc2f2eb1838f",
  "principalName": "admin@domain.contoso.com",
  "type": "User"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageSubject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
