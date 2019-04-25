---
title: appRole 资源类型
description: 表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 servicePrincipal 实体和 application 实体的**appRoles**属性是**appRole**的集合。
localization_priority: Normal
ms.openlocfilehash: 8a367406c64cf9d0d3da49716aeaf6ca3c1fa687
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535700"
---
# <a name="approle-resource-type"></a>appRole 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 [servicePrincipal](serviceprincipal.md)实体和[application](application.md)实体的**appRoles**属性是**appRole**的集合。

> 重要说明: 当前版本中禁用了此功能。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approle"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowedMemberTypes|String collection|指定是否可以通过设置为 "用户" 或将此应用程序角色定义分配给用户和组, 或通过设置为 "应用程序" 或同时设置为 "应用程序" 来将此应用程序角色定义分配给用户和组。|
|description|String|在管理员应用分配和同意体验中显示的权限帮助文本。|
|displayName|字符串|管理员同意和应用工作分配体验中显示的权限的显示名称。|
|id|Guid|**appRoles**集合中的唯一角色标识符。|
|isEnabled|Boolean|在创建或更新角色定义时, 必须将其设置为**true** (默认值)。 若要删除角色, 必须首先将此设置为**false**。  此时, 在后续调用中, 可能会删除此角色。|
|value|String|指定应用程序应在身份验证和访问令牌中预期的角色声明的值。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/approle.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
