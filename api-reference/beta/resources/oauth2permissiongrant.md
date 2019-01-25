---
title: oAuth2PermissionGrant 资源类型
description: 代表已被授予对 （由服务主体） 应用程序的 OAuth 2.0 范围 （委派权限） 为用户或管理员同意过程的一部分。
localization_priority: Normal
ms.openlocfilehash: ea6486aedca4c3fcf73e59a5652ccf517fb01ddc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516922"
---
# <a name="oauth2permissiongrant-resource-type"></a>oAuth2PermissionGrant 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表已被授予对 （由服务主体） 应用程序的 OAuth 2.0 范围 （委派权限） 为用户或管理员同意过程的一部分。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2Permissiongrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
}

```
## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|clientId|String| 服务主体的 id 授予同意以访问 （由 resourceId 属性） 的资源时模拟用户。 |
|consentType|String| 指示由 （代表组织） 管理员或个人是否提供同意。 可取值为“AllPrincipals”或“Principal”。 |
|ExpiryTime|DateTimeOffset| 目前，到期时间值将被忽略。 |
|id|String| 唯一标识符 只读。|
|principalId|String| 如果 consentType *AllPrincipals*此值为 null，并同意应用于组织中的所有用户。 如果*主体*consentType，此属性将指定的用户的授予许可，并且仅适用于该用户的 id。 |
|resourceId|String| 指定已向其授予访问的资源服务主体的 id。 |
|scope|字符串| OAuth 2.0 访问令牌中指定资源应用程序应产生预期[范围](/graph/permissions-reference)声明的值。 例如， *User.Read* |
|startTime|DateTimeOffset| 目前，开始时间值将被忽略。 |

## <a name="relationships"></a>关系
无


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |读取属性和 oAuth2PermissionGrant 对象的关系。|
|[列表 oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md)集合 | 检索 oauth2PermissionGrant 对象的列表。 |
|[更新 oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md) | [oAuth2PermissionGrant](oauth2permissiongrant.md) |更新 oAuth2PermissionGrant 对象。 |
|[删除 oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md) | 无 |删除 oAuth2PermissionGrant 对象。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/oauth2permissiongrant.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
