---
title: permissionScope 资源类型
description: 表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过 Application 对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **Oauth2Permissions**属性和应用程序实体的 ServicePrincipal 实体是**OAuth2Permission**的集合。
localization_priority: Normal
ms.openlocfilehash: 00629a6e123ef19290d3c1bd4797e4bab3ce95c0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517076"
---
# <a name="permissionscope-resource-type"></a>permissionScope 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示一个 OAuth 2.0 委派权限范围。 指定的 OAuth 2.0 委派的权限范围可能请求 （通过[Application](application.md)对象的**requiredResourceAccess**集合） 的客户端应用程序调用资源应用程序时。 **Oauth2Permissions**属性和[应用程序](application.md)实体的[ServicePrincipal](serviceprincipal.md)实体是**OAuth2Permission**的集合。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
|adminConsentDescription|String| 权限管理员同意和应用程序分配体验中显示的帮助文本。 |
|adminConsentDisplayName|String| 权限管理的同意和应用程序分配体验中显示的的显示名称。 |
|id|Guid| 唯一范围权限 oauth2Permissions 集合内的标识符。 |
|isEnabled|Boolean| 在创建或更新权限，此属性必须设置为**true** （这是默认值）。 若要删除的权限，此属性必须先设置为**false**。 此时，在后续呼叫，可能会删除权限。 |
|Origin|String| 供内部使用。 |
|type|String| 指定是否此范围权限可以同意由最终用户，或者是否必须由公司管理员同意租户级权限。 可能的值为*用户*或*管理员*。 |
|userConsentDescription|String| 权限帮助最终用户同意体验中显示的文本。 |
|userConsentDisplayName|String| 显示在最终用户同意体验中的权限的显示名称。 |
|值|String| 范围声明的资源应用程序应产生预期 OAuth 2.0 访问令牌中的值。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "adminConsentDescription": "String",
  "adminConsentDisplayName": "String",
  "id": "Guid",
  "isEnabled": true,
  "origin": "String",
  "type": "String",
  "userConsentDescription": "String",
  "userConsentDisplayName": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "permissionScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/permissionscope.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
