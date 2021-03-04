---
title: 更新 organizationalBrandingProperties
description: 更新 organizationalBrandingProperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5b3d280d2d2ac53c9775413843b9e74b1f5ff830
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447834"
---
# <a name="update-organizationalbrandingproperties"></a>更新 organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [organizationalBrandingProperties 对象](../resources/organizationalbrandingproperties.md) 的属性。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{id}/branding
PUT /organization/{id}/branding
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required.  |
| Content-Language  | 区域设置。 可选。  |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|backgroundColor|String|将出现在低带宽连接中的背景图像的颜色。 建议在此处使用横幅徽标或组织颜色的主要颜色。 以十六进制值指定 (，例如，白色#FFFFFF) 。|
|backgroundImage|Stream|显示为登录页背景的图像。 .png 或 .jpg 不大于 1920x1080 且小于 300kb。 较小的图像将降低带宽要求，使页面加载性能提高。|
|bannerLogo|Stream|显示在登录页面上的公司徽标的横幅版本。 .png 或 .jpg 不大于 36x245px。 我们建议使用透明图像，徽标周围没有填充。|
|signInPageText|String|显示在登录框底部的文本。 可以使用此信息将其他信息（如电话号码）传达给技术支持或法律声明。 此文本必须是 Unicode 且不超过 1024 个字符。|
|squareLogo|Stream|公司徽标的方形版本。 这将显示在 Windows 10 现 (OOBE) 和启用 Windows Autopilot 进行部署时。 .png 或 .jpg 大小不超过 240x240px，大小不超过 10kb。 我们建议使用透明图像，徽标周围没有填充。|
|usernameHintText|String|在登录屏幕上的用户名文本框中显示提示的字符串。 此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。|

传入时将忽略 **id** 属性。

## <a name="response"></a>响应

如果成功，此方法返回 `204 OK` 响应代码。

## <a name="examples"></a>示例
### <a name="example-1-update-default-branding"></a>示例 1：更新默认品牌
如果品牌已存在，PATCH 将仅替换指定的属性，使未指定的属性保持不变。 
#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 OK
```

在这种情况下，默认 /branding 的值会更新，但在任何本地化时不会更改任何值。

### <a name="example-2-update-bannerlogo-for-default-branding"></a>示例 2：更新默认品牌打造的 bannerLogo
以下请求更新默认品牌打造的横幅徽标。
#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-3-update-localized-branding"></a>示例 3：更新本地化品牌
如果指定了 Content-Language 标头，则创建与 Content-Language 关联的本地化（如果不存在）然后使用指定值进行更新。 默认品牌不会更改。
#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```

#### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

在此请求后，fr 本地化会使用 backgroundColor 的新值进行更新，但对默认 /branding 没有变化。

### <a name="example-4-replace-default-branding-and-all-localizations"></a>示例 4：替换默认品牌和所有本地化
如果品牌已存在，PUT 将替换默认品牌和任何本地化。
#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingProperties"
} -->

```http
HTTP/1.1 204 No Content
```

在此请求后，默认品牌仅指定了 backgroundColor，并且具有一个 id fr 的本地化，并且还设置了 backgroundColor。
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
