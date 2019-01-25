---
title: identityProvider 资源类型
description: 代表 Azure Active Directory (Azure AD) 标识提供程序。 Microsoft、 Google、 Facebook、 Amazon 或 LinkedIn，可以是标识提供程序。
localization_priority: Normal
ms.openlocfilehash: afd21635d932582f2a9ee6c2cde1cf45a9d4260f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511616"
---
# <a name="identityprovider-resource-type"></a>identityProvider 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

代表 Azure Active Directory (Azure AD) 标识提供程序。 Microsoft、 Google、 Facebook、 Amazon 或 LinkedIn，可以是标识提供程序。

Azure AD B2C 租户中配置的身份提供程序支持：

* 用户注册并使用目标应用程序中的社交帐户登录。 例如，应用程序可以使用 Azure AD B2C 允许用户使用 Facebook 帐户对服务注册。
* 用户链接现有的本地帐户向使用者应用程序中的社交帐户。 例如，用户已创建的用户名和密码 （本地帐户） 的应用程序中。 更高版本用户决定将现有的本地帐户链接到其 Facebook 帐户，以便他们可以使用 Facebook 登录。

Azure AD 租户中配置的身份提供程序使未来 B2B 来宾方案。 例如，组织有需要与 Gmail 用户共享的 Office 365 中的资源。 Gmail 用户将使用其 Google 帐户凭据进行身份验证和访问的文档。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[获取 identityProvider](../api/identityprovider-get.md) |identityProvider|读取的现有 identityProvider 属性。|
|[创建 identityProvider](../api/identityprovider-post-identityproviders.md)|identityProvider|创建新 identityProvider。|
|[更新 identityProvider](../api/identityprovider-update.md)|无|更新现有 identityProvider。|
|[删除 identityProvider](../api/identityprovider-delete.md)|无|删除现有 identityProvider。|
|[列表 identityProviders](../api/identityprovider-list.md)|identityProvider 集合|列出所有 identityProviders 配置租户中。|

## <a name="properties"></a>属性

|属性|类型|必需|可为 Null|说明|
|:---------------|:--------|:--------|:--------|:----------|
|clientId|字符串|是|否|应用程序的客户端 ID。 这是注册的标识提供程序的应用程序时所获得的客户端 ID。|
|client_secret|字符串|是|否|应用程序客户端机密。 这是注册的标识提供程序的应用程序时所获得的客户端机密。 这是只写。 读取的操作将返回"\*\*\*\*"。|
|id|字符串|否|否|标识提供程序的 ID。|
|name|String|否|否|标识提供程序的显示名称。|
|type|String|是|否|标识提供程序类型。 它必须是下列值之一： <ul><li/>Microsoft<li/>Google<li/>Amazon<li/>LinkedIn<li/>Facebook</ul>|

### <a name="where-to-get-the-client-id-and-secret"></a>了解客户端 ID 和机密

每个身份提供程序已创建应用程序注册的过程。 例如，用户创建应用程序注册与 Facebook 在[developers.facebook.com](https://developers.facebook.com/)。 生成客户端 ID 和客户端机密可以传递给[创建 identityProvider](../api/identityprovider-post-identityproviders.md)。 然后，可以对任何身份验证的租户的身份提供程序联盟的目录中的每个用户对象。 这就使用户通过身份提供程序的登录页上输入凭据来登录。 按之前租户颁发一个令牌对应用程序的 Azure AD 验证身份提供程序中的令牌。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->

```json
{
    "id": "String",
    "type": "String",
    "name": "String",
    "clientId": "String",
    "clientSecret": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/identityprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
