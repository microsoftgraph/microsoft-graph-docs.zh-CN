---
title: 创建 organizationalBrandingProperties
description: 创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 824f8344666f07376120c84877f35aacbe225b79
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447841"
---
# <a name="create-organizationalbrandingproperties"></a>创建 organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。 这将同时创建默认品牌和（可选）本地化品牌。 未为用户的浏览器语言配置本地化品牌打造集时，将加载默认品牌。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

如果组织不存在品牌，则使用 PUT 或 PATCH 为组织创建品牌。

如果已配置品牌，PUT 将覆盖所有现有值，无论请求正文中是什么。 PATCH 将仅超过请求正文中包含的值，保留未包含的值不变。

**PUT/PATCH** 上的 ID 属性将被忽略到 /branding singleton。 如果未指定 Content-Language，将创建与 ID 对应的 **默认品牌** `und` 。 如果指定了 Content-Language，则为区域设置创建品牌。
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required.  |
| Content-Language  | 区域设置。 可选。  |

## <a name="request-body"></a>请求正文

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|backgroundColor|String|将出现在低带宽连接中的背景图像的颜色。 建议在此处使用横幅徽标或组织颜色的主要颜色。 以十六进制值指定 (，例如，白色#FFFFFF) 。|
|backgroundImage|Stream|显示为登录页背景的图像。 .png 或 .jpg 不大于 1920x1080 且小于 300kb。 较小的图像将降低带宽要求，使页面加载性能提高。|
|bannerLogo|Stream|显示在登录页面上的公司徽标的横幅版本。 .png 或 .jpg 不大于 36x245px。 我们建议使用透明图像，徽标周围没有填充。|
|signInPageText|String|显示在登录框底部的文本。 可以使用此信息向技术支持或法律声明传达其他信息，例如电话号码。 此文本必须是 Unicode 且不超过 1024 个字符。|
|squareLogo|Stream|公司徽标的方形版本。 这将显示在 Windows 10 现 (OOBE) 和启用 Windows Autopilot 进行部署时。 .png 或 .jpg 大小不超过 240x240px，大小不超过 10kb。 我们建议使用透明图像，徽标周围没有填充。|
|usernameHintText|String|在登录屏幕上的用户名文本框中作为提示的字符串。 此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应代码和已创建的 `201 Created` [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。

## <a name="examples"></a>示例

以下示例为 en-US 创建默认品牌和本地化。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "signInPageText":"Welcome",
    "usernameHintText":"hint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Language: en-US

{
    "backgroundColor":"#FFFF33",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/backgroundImage",
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo",
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/bannerLogo",
    "id": "und",
    "signInPageText":"Welcome",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/squareLogo",
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/squareLogo",
    "usernameHintText":"hint"
}
```

在这种情况下，将设置默认品牌对象。 en-US 的本地化品牌设置也是由于标头中的 Content-Language 而设置的，即使响应中未返回 en-US 品牌设置。 请注意，请求中的内容语言是可选的，如果不存在，将仅设置默认品牌。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
