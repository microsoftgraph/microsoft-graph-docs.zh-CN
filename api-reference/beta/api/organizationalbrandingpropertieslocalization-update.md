---
title: 更新本地化的 organizationalbrandingproperties
description: 为特定本地化更新 organizationalbrandingproperties 对象的属性。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0b835316d611d3735a0a981fc77f58622ab89c9b
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031905"
---
# <a name="update-localized-organizationalbrandingproperties"></a>更新本地化的 organizationalbrandingproperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定本地化更新 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象的属性。

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
PATCH /organization/{id}/branding/localizations/{locale}/{property name}
PUT /organization/{id}/branding/localizations/{locale}/{property name}
```

## <a name="request-headers"></a>请求标头

| 名称       | 说明|
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required.  |
| Content-Language  | 位置. 可选。  |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|backgroundColor|String|将在低带宽连接中的背景图像处显示的颜色。 建议在此处使用横幅徽标的主要颜色或您的组织颜色。 在十六进制 (中指定此项例如，白色为 #FFFFFF) 。|
|backgroundImage|Stream|显示为登录页的背景的图像。 .png 或 .jpg 不大于1920x1080 且小于300kb。 较小的图像将降低带宽要求并使页面加载更具性能。|
|bannerLogo|Stream|显示在登录页面上的公司徽标的标题版本。 .png 或 .jpg 不大于36x245px。 我们建议使用透明图像，而不在徽标周围进行填充。|
|signInPageText|String|出现在登录框底部的文本。 您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。 此文本必须是 Unicode，且不能超过1024个字符。|
|squareLogo|Stream|公司徽标的平方版本。 在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。 .png 或 .jpg 不大于240x240px，且大小不超过10kb。 我们建议使用透明图像，而不在徽标周围进行填充。|
|usernameHintText|String|在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。 此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。|
|id|String|更新品牌的区域设置|


## <a name="response"></a>响应

如果成功，此方法返回 `204 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-setting-bannerlogo-for-the-fr-localization-using-put"></a>示例1：使用 PUT 设置用于 fr 本地化的 **bannerLogo**

以下请求更新了 fr 本地化的横幅徽标。 使用 PUT，如果不存在 fr 本地化，则返回 "找不到 404"。 如果有效负载包含 id 属性或内容语言标头，并且它们与 URL 中的 id 不匹配，则返回一个错误的请求。

#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo
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
HTTP/1.1 204 NO CONTENT
```

### <a name="example-2-update-bannerlogo-for-the-fr-localization-using-patch"></a>示例2：使用修补程序更新适用于 fr 本地化的 **bannerLogo**

以下请求更新了 fr 本地化的横幅徽标。  使用修补程序时，如果指定的本地化尚不存在，则会创建它并向其写入属性。

#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
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



### <a name="example-3-override-default-branding-value-with-a-blank-string"></a>示例3：使用空字符串替代默认品牌值

如果本地化中的属性值为 null，则将从默认品牌打造继承值。 若要避免这种情况发生，请在本地化的品牌中设置一个仅包含空格的空字符串或字符串。

#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "signInPageText": "French sign-in text.",
    "usernameHintText":" "
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

按照此请求，usernameHintText 的 fr 本地化将为空，而不是从默认品牌打造继承值。

### <a name="example-4-replace-french-localization-with-put"></a>示例4：将法语本地化替换为 PUT

若要使用 PUT 对本地化进行更新，我们应在 body 中添加所有属性以及需要更新的属性，将现有对象替换为新对象。 不在 PUT 的有效负载正文中的其他属性将设置为 NULL。 在下面的示例中，仅保留 backgroundColor 属性并更新 signInPageText，而将其他设置为 null。
如果指定的本地化尚不存在，则放置到指定本地化创建该的 URL。
如果有效负载包含 id 属性或内容语言标头，并且它们与 URL 中的 id 不匹配，则会引发错误的请求。

#### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandingproperties"
}-->

```http
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "fr"
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update organizationalbrandingproperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->