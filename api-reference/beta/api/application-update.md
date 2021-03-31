---
title: 更新应用程序
description: 更新 application 对象的属性。
author: sureshja
localization_priority: Normal
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 0b27abb758a52fd591540f3da54079478409f1da
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473267"
---
# <a name="update-application"></a>更新应用程序

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 application [对象的属性](../resources/application.md) 。

> [!IMPORTANT]
> 不支持使用 PATCH 设置 [**passwordCredential**](../resources/passwordcredential.md)。 使用 [addPassword](./application-addpassword.md) 和 [removePassword](./application-removepassword.md) 方法更新应用程序的密码。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Application.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
|委派（个人 Microsoft 帐户） | Application.ReadWrite.All    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:----------|
| Authorization | Bearer {token}。必需。  |
| Content-Type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性                | 类型                                                                        | 说明                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:------------------------|:----------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| api                     | [apiApplication](../resources/apiapplication.md)                            | 指定实现 Web API 的应用程序的设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| appRoles                | [appRole](../resources/approle.md) 集合                               | 应用程序可声明的应用程序角色的集合。 这些角色可以分配给用户、组或服务主体。 不可为空。                                                                                                                                                                                                                                                                                                                                                                                                                |
| displayName             | String                                                                      | 应用程序的显示名称。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| groupMembershipClaims   | String                                                                      | 配置 **应用程序期望** 的用户或 OAuth 2.0 访问令牌中颁发的组声明。 要设置此属性，请使用以下有效字符串值之一：<ul><li>`None`</li><li>`SecurityGroup`：对于安全组和 Azure Active Directory (Azure AD) 角色</li><li>`All`：该操作可获取登录用户所属的所有安全组、通讯组和 Azure AD 目录角色</li></ul>                                                                                                                       |
| identifierUris          | String collection                                                           | URI，用于在应用程序的 Azure AD 租户中标识该应用程序；如果应用程序是多租户的，则用于在已验证的自定义域中标识该应用程序。 有关详细信息，请参阅[应用程序对象和服务主体对象](/azure/active-directory/develop/app-objects-and-service-principals)。 需要多值属性筛选器表达式的 *any* 运算符。 不可为 Null。                                                                                                                                                 |
| info                    | [informationalUrl](../resources/informationalurl.md)                        | 应用程序的基本个人资料信息，例如应用的营销、支持、服务条款和隐私声明 URL。 服务条款和隐私声明通过用户同意体验展示给用户。 有关详细信息，请参阅为注册的 [Azure AD](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)应用添加服务条款和隐私声明。                                                                                                                       |
| isFallbackPublicClient  | Boolean                                                                     | 将回退应用程序类型指定为公共客户端，例如在移动设备上运行的已安装应用程序。 默认值为 `false` ，这意味着回退应用程序类型是机密客户端，如 Web 应用。 在某些情况下，Azure AD 无法确定客户端应用程序类型 (例如 [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) 流，其中配置客户端应用程序类型时未指定重定向 URI) 。 在这种情况下，Azure AD 将基于此属性的值解释应用程序类型。 |
| keyCredentials          | [keyCredential](../resources/keycredential.md) 集合                   | 与应用程序关联的密钥凭据集合。 不可为空。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| logo                    | Stream                                                                      | 应用程序的主徽标。 不可为空。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| onPremisesPublishing    | [onPremisesPublishing](../resources/onpremisespublishing.md)                | 表示用于为本地应用程序配置 [Azure AD 应用程序](https://aka.ms/whyappproxy) 代理的属性集。 此属性只能在创建应用程序后设置。                                                                                                                                                                                                                                                                                                                                                       |
| optionalClaims          | optionalClaims                                                              | 应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。 有关详细信息 [，请参阅](/azure/active-directory/develop/active-directory-optional-claims) 可选声明。                                                                                                                                                                                                                                     |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md)          | 指定应用程序的家长控制设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| publicClient            | [publicClientApplication](../resources/publicclientapplication.md)          | 指定已安装客户端（如台式设备或移动设备）的设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| requiredResourceAccess  | [requiredResourceAccess](../resources/requiredresourceaccess.md) 集合 | 指定此应用程序需要访问的资源以及在每个资源下所需的 OAuth 权限范围和应用程序角色集。 这种预配置的所需资源访问权限可驱动同意体验。 不可为 Null。                                                                                                                                                                                                                                                                                                 |
| signInAudience          | String                                                                      | 指定当前应用程序支持的 Microsoft 帐户。 支持的值为：<ul><li>`AzureADMyOrg`：在我的组织的 Azure AD 租户（即单租户）中拥有 Microsoft 工作或学校帐户的用户</li><li>`AzureADMultipleOrgs`：在任何组织的 Azure AD 租户（即多租户）中拥有 Microsoft 工作或学校帐户的用户</li> <li>`AzureADandPersonalMicrosoftAccount`：拥有个人 Microsoft 帐户或任意组织的 Azure AD 租户中的工作或学校帐户的用户</li></ul>                           |
| tags                    | String 集合                                                           | 可用于分类和标识应用程序的自定义字符串。 不可为空。                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| tokenEncryptionKeyId    | String                                                                      | 指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 将使用此属性指向的密钥对其发出的所有令牌进行加密。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。                                                                                                                                                                                                                               |
| uniqueName | String | 可作为备用标识符分配给应用程序的唯一标识符。 不可变。 只读。 |
| web                     | [webApplication](../resources/webapplication.md)                            | 指定 Web 应用程序的设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | 指定单页应用程序的设置，包括注销 URL 并重定向授权代码和访问令牌的 URI。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码，不会在响应正文中返回任何内容。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json
Content-length: 72

{
  "displayName": "New display name"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->



