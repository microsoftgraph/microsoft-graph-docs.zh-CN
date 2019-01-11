---
title: 更新 serviceprincipal
description: 更新 serviceprincipal 对象的属性。
localization_priority: Normal
ms.openlocfilehash: a8d4eebe64ac9c0c658ae9c43e2e92045be67424
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27813025"
---
# <a name="update-serviceprincipal"></a>更新 serviceprincipal

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

更新 serviceprincipal 对象的属性。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Application.ReadWrite.OwnedBy Application.ReadWrite.All |

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
|accountEnabled|布尔|                **true**如果已启用的服务主体帐户;否则为**false**。            |
|appDisplayName|字符串|通过关联的应用程序公开的显示名称。|
|appId|String|关联的应用程序 （其**appId**属性） 的唯一标识符。|
|appRoleAssignmentRequired|布尔|指定 Azure AD 将问题的用户或访问令牌对应用程序之前是否需要向用户或组**appRoleAssignment** 。                            **说明**： 需要 1.5 版或更高版本，不可为空。            |
|appRoles|appRole|由关联的应用程序公开应用程序角色。 有关详细信息看到**appRoles**属性定义应用程序实体**注释**： 需要 1.5 版或更高版本，不可为空。            |
|displayName|字符串|服务主体的显示名。|
|errorUrl|字符串|            |
|主页|字符串|关联的应用程序的主页的 URL。|
|keyCredentials|keyCredential|关键凭据与主体服务相关联的集合。                            **注意：** 不可为 null。            |
|logoutUrl|字符串| 指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。 |
|oauth2Permissions|oAuth2Permission|由关联的应用程序公开 OAuth 2.0 权限。 有关详细信息请参阅应用程序在实体上的**oauth2Permissions**属性定义。                            **说明**： 需要 1.5 版或更高版本，不可为空。            |
|passwordCredentials|passwordCredential|密码凭据的服务主体相关联的集合。                            **注意：** 不可为 null。            |
|preferredTokenSigningKeyThumbprint|字符串|保留以仅供内部使用。 不要编写或否则依赖于此属性。 可能会在将来版本中删除。                            **说明**： 要求 1.5 或更高版本。            |
|publisherName|String|在其中指定关联的应用程序租户的显示名称。|
|replyUrls|字符串|用户令牌发送到的登录关联的应用程序或重定向 Uri 的 OAuth 2.0 授权代码和访问令牌发送到关联的应用程序的 Url。                            **注意：** 不可为 null。            |
|samlMetadataUrl|字符串|            |
|servicePrincipalNames|字符串|标识关联的应用程序的 Uri。 有关详细信息，请参阅[应用程序对象和服务主体对象](https://msdn.microsoft.com/library/azure/dn132633.aspx)。                            **说明**： 不可为空， **any**运算符，则需要为多值属性; 筛选器表达式有关详细信息，请参阅[支持的查询，筛选器和分页选项](https://msdn.microsoft.com/library/azure/dn727074.aspx)。            |
|标记前添加的标记|String|                                        **注意：** 不可为 null。            |

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
<!-- {
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
