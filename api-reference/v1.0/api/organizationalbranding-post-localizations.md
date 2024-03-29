---
title: 创建 organizationalBrandingLocalization
description: 创建新的组织BrandingLocalization 对象。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8a2bba2591aefa4bc5dfd5821f8358af66e82dc3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439248"
---
# <a name="create-organizationalbrandinglocalization"></a>创建 organizationalBrandingLocalization
命名空间：microsoft.graph

创建新的 [组织BrandingLocalization](../resources/organizationalBrandingLocalization.md) 对象。 这会创建一个本地化品牌，同时，如果不存在，则创建默认品牌。

默认品牌创建仅一次。 如果未为用户的浏览器语言配置本地化品牌，则会加载它。 若要检索默认品牌，请参阅 [Get 品牌](organizationalbranding-get.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
此请求创建新的本地化品牌和默认品牌（如果尚不存在）。 
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/branding/localizations
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

下表显示了创建 [组织BrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| id | String | 一个标识符，表示使用区域性名称指定的区域设置。 区域性名称遵循 RFC 1766 标准，格式为“languagecode2-country/regioncode2”，其中“languagecode2”是派生自 ISO 639-1 的小写双字母代码，“country/regioncode2”是派生自 ISO 3166 的大写双字母代码。 例如，美国英语是 `en-US`. 无法通过将 **ID** 的值设置为字符串类型或`default`字符串类型`0`来创建默认品牌。  <br/><br/>**注意：** 目前不支持单个区域设置的多个品牌。 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [组织BrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象。

## <a name="examples"></a>示例

以下示例为法语 () `fr-FR` 本地化创建品牌本地化。 String 类型的任何未指定属性都继承自默认品牌对象中的值。 例如，如果默认品牌对象中的 signInPageText 为 `null`，则此请求中创建的品牌的 signInPageText `fr-FR` 也将为 `null`。 若要重写 `null` 不带任何文本的值，请使用仅包含空格的字符串。

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandinglocalization"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr-FR",
    "signInPageText": " "
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-organizationalbrandinglocalization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-organizationalbrandinglocalization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-organizationalbrandinglocalization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-organizationalbrandinglocalization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-organizationalbrandinglocalization-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-organizationalbrandinglocalization-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')/branding/localizations/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/directoryObjects/$/Microsoft.DirectoryServices.Organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')//localizations/fr-FR",
    "id": "fr-FR",
    "backgroundColor": "",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": null,
    "cdnList": [],
    "signInPageText": " ",
    "squareLogoRelativeUrl": null,
    "usernameHintText": ""
}
```
