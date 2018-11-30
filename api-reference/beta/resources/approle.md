---
title: appRole 资源类型
description: 表示应用程序角色调用另一个应用程序的客户端应用程序可能请求的或可能用于分配给用户或组指定的应用程序角色中的应用程序。 **AppRoles**属性和应用程序实体的 servicePrincipal 实体是**appRole**的集合。
ms.openlocfilehash: f87ef6f40fbeb18ec4b3a2373fb2a19e14da84a4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042921"
---
# <a name="approle-resource-type"></a>appRole 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示应用程序角色调用另一个应用程序的客户端应用程序可能请求的或可能用于分配给用户或组指定的应用程序角色中的应用程序。 **AppRoles**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**appRole**的集合。

> 重要说明： 此功能在当前版本中已禁用。

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
|allowedMemberTypes|String 集合|指定此应用程序角色定义可以设置为"User"，或其他应用程序 （即正在访问此端口监控程序服务方案中的应用程序） 分配给用户和组设置到"应用程序"，或两者。|
|说明|字符串|权限帮助管理应用程序分配中显示的文本和同意体验。|
|displayName|字符串|权限管理的同意和应用程序分配体验中显示的的显示名称。|
|id|Guid|**AppRoles**集合内的独有角色标识符。|
|isEnabled|Boolean|当创建或更新一个角色定义，这必须设置为**true** （这是默认值）。 若要删除一个角色，这必须先设置为**false**。  此时，在后续呼叫，可以删除此角色。|
|值|字符串|身份验证和访问令牌中指定应用程序应产生预期角色声明的值。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->