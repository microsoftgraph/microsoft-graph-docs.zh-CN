---
title: permissionScope 资源类型
description: 表示 OAuth 2.0 委派的权限范围。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: be8d9a7d08334bd716cfcbf565225add790b65e3
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939367"
---
# <a name="permissionscope-resource-type"></a>permissionScope 资源类型

表示 OAuth 2.0 委派的权限范围。 调用资源应用程序时，客户端应用程序可能会请求指定的 OAuth 2.0 委派权限范围（通过[application](application.md)对象上的**requiredResourceAccess**集合）。 **Oauth2Permissions**属性 <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> [应用程序](application.md)实体是**permissionScope**的集合。

## <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
|:---------------|:--------|:----------|
|adminConsentDescription|String| 管理员同意和应用工作分配体验中显示的权限帮助文本。 |
|adminConsentDisplayName|String| 管理员同意和应用工作分配体验中显示的权限的显示名称。 |
|id|Guid| Oauth2Permissions 集合中的唯一作用域权限标识符。 |
|isEnabled|Boolean| 在创建或更新权限时，此属性必须设置为**true** （默认值）。 若要删除权限，必须首先将此属性设置为**false**。 此时，在后续调用中，可能会删除该权限。 |
|格式|String| 供内部使用。 |
|type|String| 指定此范围权限是否可由最终用户许可，或者是否为公司管理员必须同意的租户范围内的权限。 可能的值为*User*或*Admin*。 |
|userConsentDescription|String| 最终用户同意体验中显示的权限帮助文本。 |
|userConsentDisplayName|String| 显示在最终用户同意体验中的权限的显示名称。 |
|value|String| 在 OAuth 2.0 访问令牌中，资源应用程序应期望的范围声明的值。 |

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
  "suppressions": []
}
-->
