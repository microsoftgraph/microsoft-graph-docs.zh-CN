---
title: 更新 organizationalBrandingProperties
description: 更新 organizationalBrandingProperties 对象的属性。
localization_priority: Normal
author: AlexanderMars
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bd400c50fc6a51e80ccfadc6cfbb1c6e655f53ea
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680757"
---
# <a name="update-organizationalbrandingproperties"></a>更新 organizationalBrandingProperties

更新 [organizationalBrandingProperties 对象](../resources/organizationalbrandingproperties.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /organization/{tenant id}/branding/{property name}
PUT /organization/{tenant id}/branding/{property name}
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
|backgroundColor|String|将出现在低带宽连接中的背景图像上的颜色。 建议在此处使用横幅徽标或组织颜色的主要颜色。 以十六进制表示 (，例如，白色#FFFFFF) 。|
|backgroundImage|Stream|显示为登录页背景的图像。 .png或 .jpg不超过 1920x1080 且小于 300kb。 较小的图像将降低带宽要求，提高页面加载性能。|
|bannerLogo|Stream|显示在登录页上的公司徽标的横幅版本。 .png或.jpg不超过 36x245px。 我们建议使用透明图像，徽标周围没有填充。|
|signInPageText|String|显示在登录框底部的文本。 您可以使用此信息来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须是 Unicode 且不超过 1024 个字符。|
|squareLogo|Stream|公司徽标的方形版本。 这将显示在 Windows 10 现成 (OOBE) 以及启用 Windows Autopilot 进行部署时。 .png或 .jpg不超过 240x240px 且大小不超过 10kb。 我们建议使用透明图像，徽标周围没有填充。|
|usernameHintText|String|字符串，在登录屏幕的用户名文本框中作为提示显示。 此文本必须是 Unicode，不带链接或代码，并且不能超过 64 个字符。|

传入时将忽略 **id** 属性。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例
### <a name="example-1-update-default-branding"></a>示例 1：更新默认品牌
如果品牌已存在，将 `PATCH` 仅替换指定的属性，不更改未指定的属性。 
#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_1"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-1-java-snippets.md)]
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

在这种情况下，将更新默认品牌设置的值，但任何本地化时不会更改任何值。

### <a name="example-2-update-bannerlogo-for-default-branding"></a>示例 2：为默认品牌更新 bannerLogo
以下请求更新默认品牌打造的横幅徽标。
#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_2"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
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

### <a name="example-3-update-localized-branding"></a>示例 3：更新本地化品牌
如果 **指定了 Content-Language** 标头，则首先创建与 **Content-Language** 关联的本地化（如果它不存在的话）然后使用指定的值进行更新。 默认品牌不会更改。
#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_3"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
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

在此请求后， `fr` 本地化会使用 **backgroundColor** 的新值进行更新，但对默认品牌没有任何更改。

### <a name="example-4-replace-default-branding-and-all-localizations"></a>示例 4：替换默认品牌和所有本地化
如果品牌已存在， `PUT` 将替换默认品牌和任何本地化。
#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties_4"
}-->

```http
PUT https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Content-Language: fr

{
    "backgroundColor":"#FFFF33"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandingproperties-4-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandingproperties-4-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandingproperties-4-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandingproperties-4-java-snippets.md)]
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

在此请求之后，默认品牌仅指定了 **backgroundColor，** 并且具有 id 以及 `fr` **backgroundColor** 集的完全一个本地化。
<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
