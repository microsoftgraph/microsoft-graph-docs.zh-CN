---
title: 更新应用程序
description: 更新应用程序对象的属性。
author: sureshja
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5eca1c3b8455bc2b9ba9694a7beb4b2f1132e84f
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670328"
---
# <a name="update-application"></a>更新应用程序

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [应用程序](../resources/application.md) 对象的属性。

> [!IMPORTANT]
> 不支持使用 PATCH 设置 [**passwordCredential**](../resources/passwordcredential.md)。 使用 [addPassword](./application-addpassword.md) 和 [removePassword](./application-removepassword.md) 方法更新应用程序的密码或机密。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  Application.ReadWrite.All、Directory.ReadWrite.All |
|委派（个人 Microsoft 帐户） | Application.ReadWrite.All    |
|应用程序 | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
将 `{id}` 替换为应用程序对象的 **ID**，在 Azure 门户中也称为 **对象 ID**。
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
| groupMembershipClaims   | String                                                                      | 配置应用程序所需的用户或 OAuth 2.0 访问令牌中颁发的 **组** 声明。 要设置此属性，请使用以下有效字符串值之一：<ul><li>`None`</li><li>`SecurityGroup`：对于安全组和 Azure Active Directory (Azure AD) 角色</li><li>`All`：该操作可获取登录用户所属的所有安全组、通讯组和 Azure AD 目录角色</li></ul>                                                                                                                       |
| identifierUris          | String collection                                                           | URI，用于在应用程序的 Azure AD 租户中标识该应用程序；如果应用程序是多租户的，则用于在已验证的自定义域中标识该应用程序。 有关详细信息，请参阅[应用程序对象和服务主体对象](/azure/active-directory/develop/app-objects-and-service-principals)。 需要多值属性筛选器表达式的 *any* 运算符。 不可为 Null。                                                                                                                                                                           |
| info                    | [informationalUrl](../resources/informationalurl.md)                        | 应用程序的基本配置文件信息，例如应用的营销、支持、服务条款和隐私声明 URL。 服务条款和隐私声明通过用户同意体验展示给用户。 有关详细信息，请参阅 [已注册 Azure AD 应用的“添加服务条款”和隐私声明](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement)。                                                                                                                                                 |
| isFallbackPublicClient  | Boolean                                                                     | 将回退应用程序类型指定为公共客户端，例如在移动设备上运行的已安装应用程序。 默认值为 `false`，这意味着回退应用程序类型是机密客户端，如 Web 应用。 在某些情况下，Azure AD 无法确定客户端应用程序类型 (例如 [，在不](https://tools.ietf.org/html/rfc6749#section-4.3) 指定重定向 URI) 的情况下配置该应用程序类型的 ROPC 流。 在这些情况下，Azure AD 将根据此属性的值解释应用程序类型。 |
| keyCredentials          | [keyCredential](../resources/keycredential.md) 集合                   | 与应用程序关联的密钥凭据集合。不可为 Null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| logo                    | Stream                                                                      | 应用程序的主徽标。不可为 Null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| onPremisesPublishing    | [onPremisesPublishing](../resources/onpremisespublishing.md)                | 表示用于为本地应用程序配置 [Azure AD 应用程序代理](/azure/active-directory/app-proxy/what-is-application-proxy)的属性集。 此属性只能在创建应用程序后设置，并且不能在与其他应用程序属性相同的请求中更新。                                                                                                                                                                                                                                                                                                                                                       |
| optionalClaims          | optionalClaims                                                              | 应用程序开发人员可以在其 Azure AD 应用中配置可选声明，以指定 Microsoft 安全令牌服务发送到他们应用程序的令牌中所需的声明。 有关详细信息，请参阅 [可选声明](/azure/active-directory/develop/active-directory-optional-claims) 。                                                                                                                                                                                                                                                               |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md)          | 指定应用程序的家长控制设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| publicClient            | [publicClientApplication](../resources/publicclientapplication.md)          | 指定已安装客户端（如台式设备或移动设备）的设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| requiredResourceAccess  | [requiredResourceAccess](../resources/requiredresourceaccess.md) 集合 | 指定应用程序需要访问的资源。 此属性还指定每个资源所需的委派权限和应用程序角色的集合。 该配置对所需的资源的访问将推动许可体验。 可配置的资源服务 (API) 不能超过 50 个。 从 2021 年 10 月中旬开始，所需权限总数不得超过 400 个。 不可为空。                                                                                                                 |
| samlMetadataUrl | String | 服务用于公开联合身份验证的 SAML 元数据的 URL。 此属性仅对单租户应用程序有效。 |
| signInAudience          | String                                                                      | 指定当前应用程序支持的 Microsoft 帐户。 支持的值为：<ul><li>`AzureADMyOrg`：在我的组织的 Azure AD 租户（即单租户）中拥有 Microsoft 工作或学校帐户的用户</li><li>`AzureADMultipleOrgs`：在任何组织的 Azure AD 租户（即多租户）中拥有 Microsoft 工作或学校帐户的用户</li> <li>`AzureADandPersonalMicrosoftAccount`：拥有个人 Microsoft 帐户或任意组织的 Azure AD 租户中的工作或学校帐户的用户</li></ul>                           |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | 指定单页应用程序的设置，包括注销 URL 并重定向授权代码和访问令牌的 URI。 |
| 标记                    | 字符串集合                                                           | 可用于分类和标识应用程序的自定义字符串。不可为 null。                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| tokenEncryptionKeyId    | String                                                                      | 指定 keyCredentials 集合中的公共密钥的 keyId。 配置后，Azure AD 将使用此属性指向的密钥对其发出的所有令牌进行加密。 接收加密令牌的应用程序代码必须先使用匹配的私钥来解密该令牌，然后才能将该令牌用于登录用户。                                                                                                                                                                                                                               |
| 唯一名称 | String | 可指定给应用程序作为替代标识符的唯一标识符。不可变。只读。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| web                     | [webApplication](../resources/webapplication.md)                            | 指定 Web 应用程序的设置。                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | 指定单页应用程序的设置，包括注销 URL 并重定向授权代码和访问令牌的 URI。 |
| windows                     | [windowsApplication](../resources/windowsapplication.md)                            | 指定运行 Microsoft Windows 并在 Microsoft Store 或 Xbox 游戏商店中发布的应用的设置。 包括用于授权代码和访问令牌的包 SID 和重定向 URI。 |

## <a name="response"></a>响应

如果成功，此方法将返回 `204 No Content` 响应代码，并且不会在响应正文中返回任何内容。
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-application-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-application-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

<!-- {
  "blockType": "response"
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
