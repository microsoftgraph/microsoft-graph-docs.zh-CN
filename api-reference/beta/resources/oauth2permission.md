---
title: oAuth2Permission 资源类型
description: 表示 OAuth 2.0 委派的权限范围。 调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过 application 对象上的**requiredResourceAccess**集合）。 ServicePrincipal 实体和 application 实体的**appRoles**属性是**oAuth2Permission**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 6acbf07ae6212a68519cbbf44a2730ac3b90e4b9
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200143"
---
# <a name="oauth2permission-resource-type"></a>oAuth2Permission 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 OAuth 2.0 委派的权限范围。 调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过[application](application.md)对象上的**requiredResourceAccess**集合）。 [ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**appRoles**属性是**oAuth2Permission**的集合。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permission"
}-->

```json
{
  "adminConsentDescription": "string",
  "adminConsentDisplayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "type": "string",
  "userConsentDescription": "string",
  "userConsentDisplayName": "string",
  "value": "string"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|adminConsentDescription|字符串|管理员同意和应用工作分配体验中显示的权限帮助文本。|
|adminConsentDisplayName|字符串|管理员同意和应用工作分配体验中显示的权限的显示名称。|
|id|Guid|Oauth2Permissions 集合中的唯一作用域权限标识符。|
|isEnabled|Boolean|在创建或更新权限时，此属性必须设置为**true** （默认值）。 若要删除权限，必须首先将此属性设置为**false**。  此时，在后续调用中，可能会删除该权限。|
|type|字符串|指定此范围权限是否可由最终用户许可，或者是否为公司管理员必须同意的租户范围内的权限。  可能的值为 "User" 或 "Admin"。|
|userConsentDescription|字符串|最终用户同意体验中显示的权限帮助文本。|
|userConsentDisplayName|字符串|最终用户同意体验中显示的权限的显示名称。|
|value|String|在 OAuth 2.0 访问令牌中，资源应用程序应期望的范围声明的值。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
