---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641174"
---
# <a name="update-serviceprincipal"></a>更新 serviceprincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 serviceprincipal 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 类型 | 说明|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。

| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean|                如果服务主体帐户已启用，则为 **true**；否则，为 **false**。            |
|appDisplayName|String|关联应用程序公开的显示名称。|
|appId|String|关联应用程序的唯一标识符（其 **appId** 属性）。|
|appRoleAssignmentRequired|Boolean|指定在 Azure AD 在向应用程序签发用户或访问令牌之前用户或组是否需要 **appRoleAssignment**。                            **说明**： 需要 1.5 版或更高版本，不可为空。            |
|appRoles|appRole|关联应用程序公开的应用程序角色。 有关详细信息看到**appRoles**属性定义应用程序实体**注释**： 需要 1.5 版或更高版本，不可为空。            |
|displayName|String|服务主体的显示名称。|
|errorUrl|String|            |
|homepage|String|关联的应用程序的主页的 URL。|
|keyCredentials|keyCredential|与服务帐户关联的密钥凭据集合。                            **注意：** 不可为 null。            |
|logoutUrl|String| 指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。 |
|oauth2Permissions|oAuth2Permission|关联应用程序的 OAuth 2.0 权限。 有关详细信息，请参阅应用程序实体上的 **oauth2Permissions** 属性定义。                            **说明**： 需要 1.5 版或更高版本，不可为空。            |
|passwordCredentials|passwordCredential|与服务帐户关联的密码凭据集合。                            **注意：** 不可为 null。            |
|preferredTokenSigningKeyThumbprint|String|仅供内部使用。 请勿写入属性，否则将依赖该属性。 可能会在未来版本中删除。                            **说明**： 要求 1.5 或更高版本。            |
|publisherName|String|在其中指定关联应用程序的租户的显示名称。|
|replyUrls|String|向其发送用户令牌以使用关联应用程序登录的 URL，或者为关联应用程序向其发送 OAuth 2.0 authorization 代码和访问令牌的重定向 URL。                            **注意：** 不可为 null。            |
|samlMetadataUrl|String|            |
|servicePrincipalNames|String|标识关联应用程序的 URL。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。                            **说明**： 不可为空， **any**运算符，则需要为多值属性; 筛选器表达式有关详细信息，请参阅[支持的查询，筛选器和分页选项](https://msdn.microsoft.com/library/azure/dn727074.aspx)。            |
|tags|String|                                        **注意：** 不可为 null。            |

## <a name="response"></a>响应

如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[servicePrincipal](../resources/serviceprincipal.md)对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.serviceprincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
