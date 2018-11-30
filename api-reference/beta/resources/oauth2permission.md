---
title: oAuth2Permission 资源类型
description: 表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过 application 对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **AppRoles**属性和应用程序实体的 servicePrincipal 实体是**oAuth2Permission**的集合。
ms.openlocfilehash: 4a790c935dd84fb7bd4e1422ca59914d9a319ae9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046965"
---
# <a name="oauth2permission-resource-type"></a>oAuth2Permission 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过[application](application.md)对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **AppRoles**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**oAuth2Permission**的集合。


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
|adminConsentDescription|字符串|权限管理员同意和应用程序分配体验中显示的帮助文本。|
|adminConsentDisplayName|字符串|权限管理的同意和应用程序分配体验中显示的的显示名称。|
|id|Guid|唯一范围权限 oauth2Permissions 集合内的标识符。|
|isEnabled|Boolean|在创建或更新权限，此属性必须设置为**true** （这是默认值）。 若要删除的权限，此属性必须先设置为**false**。  此时，在后续呼叫，可能会删除权限。|
|type|字符串|指定是否此范围权限可以同意由最终用户，或者是否必须同意公司管理员通过租户级权限。  可能的值为"用户"或"管理员"。|
|userConsentDescription|字符串|权限帮助最终用户同意体验中显示的文本。|
|userConsentDisplayName|字符串|显示在最终用户同意体验中的权限的显示名称。|
|值|字符串|范围声明的资源应用程序应产生预期 OAuth 2.0 访问令牌中的值。|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
