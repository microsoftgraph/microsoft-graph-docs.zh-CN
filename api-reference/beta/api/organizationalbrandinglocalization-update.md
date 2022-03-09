---
title: 更新 organizationalBrandingLocalization
description: 更新 organizationalBrandingLocalization 对象的属性。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5544a1aba05fd97fbc8c45e5915491fc11eed916
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63397615"
---
# <a name="update-organizationalbrandinglocalization"></a>更新 organizationalBrandingLocalization
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定本地化 [更新 organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

使用 PUT 方法仅更新 Stream 数据类型，包括 **backgroundLogo** 和 **backgroundImage**。 若要更新 String 数据类型（包括 **signInPageText** 和 **usernameHintText**），请使用 PATCH 方法。 不能在同一请求中用其他数据类型更新 Stream 类型。

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
PUT /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}/{backgroundImage | bannerLogo | squareLogo}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| backgroundColor | String | 在低带宽连接中显示的颜色，用于表示背景图像。 我们建议你使用横幅徽标的主要颜色或你的组织颜色。 以十六进制格式指定此参数，例如，white 为 `#FFFFFF`。 |
| backgroundImage | Stream | 显示为登录页背景的图像。 允许的类型是 PNG 或 JPEG，不小于 300 KB 且不超过 1920 × 1080 像素。 较小的图像将降低带宽要求，并加快页面加载速度。 |
| bannerLogo | Stream | 显示在登录页上的公司徽标的横幅版本。 允许的类型是 PNG 或 JPEG，不超过 36 × 245 像素。 我们建议使用透明图像，徽标周围没有填充。 |
| customAccountResetCredentialsUrl | String | 用于重置帐户凭据的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 |
| customCannotAccessYourAccountText | 字符串 | 一个字符串，用于替换默认字符串"无法访问你的帐户？" 自助密码重置 (SSPR) 登录页面上的超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customForgotMyPasswordText | 字符串 | 一个字符串，用于替换登录表单上的默认"忘记密码"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customPrivacyAndCookiesText | String | 一个字符串，用于替换页脚中的默认"隐私和 Cookie"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customPrivacyAndCookiesUrl | 字符串 | 用于替换页脚中"隐私和 Cookie"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 |
| customTermsOfUseText | 字符串 | 一个字符串，用于替换页脚中的默认"使用条款"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customTermsOfUseUrl | String | 用于替换页脚中"使用条款"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，并且不得超过 128 个字符。 |
| favicon | Stream | 自定义图标 (替换) 租户上的默认 Microsoft 产品Azure AD图标。 |
| headerBackgroundColor | 字符串 | 要应用以自定义页眉颜色的 RGB 颜色。 |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | 表示可在租户的登录页上隐藏的各种文本。 所有属性都可以更新。 |
| signInPageText | String | 显示在登录框底部的文本。 使用它来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须采用 Unicode 格式，且不得超过 1024 个字符。 |
| squareLogo | Stream | 在 OOBE Windows 10 OOBE (中显示公司徽标的正方形) ，Windows Autopilot 启用部署。 允许的类型是 PNG 或 JPEG，其大小不超过 240 x 240 像素且大小不超过 10 KB。 我们建议使用透明图像，徽标周围没有填充。|
| usernameHintText | String | 一个字符串，在登录屏幕的用户名文本框中作为提示显示。 此文本必须是不带链接或代码的 Unicode，并且不能超过 64 个字符。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-setting-bannerlogo-for-the-fr-fr-localization-using-put"></a>示例 1：使用 PUT 为 fr-FR 本地化设置 **bannerLogo**

以下请求更新 fr-FR 本地化的横幅徽标。

#### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-the-backgroundcolor-and-signinpagetext-for-the-fr-fr-localization-using-patch"></a>示例 2：使用 PATCH 更新 fr-FR 本地化的 backgroundColor 和 signInPageText

以下请求更新本地化的横幅 `fr-FR` 徽标。

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization6"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "Welcome to Contoso France"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocalization6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocalization6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocalization6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocalization6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization6-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-a-default-branding-value-with-a-blank-string"></a>示例 3：使用空字符串替代默认品牌值

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization7"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "signInPageText": "Welcome to Contoso France.",
    "usernameHintText":" "
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocalization7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocalization7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocalization7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocalization7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization7-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

请求后，本地化的 **usernameHintText** `fr-FR` 将为空，而不是从默认品牌对象继承值。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
