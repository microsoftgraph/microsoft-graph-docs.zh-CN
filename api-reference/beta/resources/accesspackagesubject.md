---
title: accessPackageSubject 资源类型
description: 在 Azure AD 权利管理中，访问包分配的主题。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0adfca021ec463029a4b35c047ac85f8ce52921b
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467055"
---
# <a name="accesspackagesubject-resource-type"></a>accessPackageSubject 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [Azure AD 权利](entitlementmanagement-root.md)管理中，访问包主题是可配置为请求或分配访问包的用户、服务主体或其他实体。  它可以表示来自尚未在租户中的已连接组织的请求者。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|displayName|String|主题显示名称。|
|email|String|主题的电子邮件地址。|
|id|String| 只读。|
|objectId|String|主题的对象标识符。 `null` 如果主题不是租户中的用户。|
|principalName|String|主题的主体名称（如果已知）。|
|type|String|主题的资源类型。|
|connectedOrganizationId|String|主题的已连接组织的标识符。|

## <a name="relationships"></a>关系

| 关系 | 类型        | 说明 |
|:-------------|:------------|:------------|
|connectedOrganization|[connectedOrganization](connectedorganization.md)| 主题的已连接组织。 只读。 可为 Null。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageSubject",
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

