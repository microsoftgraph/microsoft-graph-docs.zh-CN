---
title: 更新 organizationalBrandingLocalization
description: 更新组织BrandingLocalization 对象的属性。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8fa2a1eb9f22c1055bb99666f4845a3a8505ffe0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443305"
---
# <a name="update-organizationalbrandinglocalization"></a>更新 organizationalBrandingLocalization
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [组织BrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象的属性以进行特定的本地化。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

仅使用 PUT 方法更新流数据类型，包括 **backgroundLogo** 和 **backgroundImage**。 若要更新字符串数据类型（包括 **signInPageText** 和 **usernameHintText**），请使用 PATCH 方法。 不能在同一请求中使用其他数据类型更新流类型。

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
| backgroundColor | String | 显示在低带宽连接中代替背景图像的颜色。 建议使用横幅徽标或组织颜色的主要颜色。 以十六进制格式指定此值，例如，白色为 `#FFFFFF`。 |
| backgroundImage | Stream | 显示为登录页背景的图像。 允许的类型是 PNG 或 JPEG，不小于 300 KB，不大于 1920 × 1080 像素。 较小的图像将减少带宽要求，并加快页面加载速度。 |
| bannerLogo | Stream | 登录页上显示的公司徽标的横幅版本。 允许的类型为不大于 36 × 245 像素的 PNG 或 JPEG。 建议使用不填充徽标的透明图像。 |
| customAccountResetCredentialsUrl | String | 用于重置帐户凭据的自定义 URL。 此 URL 必须采用 ASCII 格式，否则非 ASCII 字符必须进行 URL 编码，且不超过 128 个字符。 |
| customCannotAccessYourAccountText | String | 一个字符串，用于替换默认的“无法访问你的帐户？” SSPR (自助密码重置) 登录页上的超链接文本。 此文本必须采用 Unicode 格式，且不超过 256 个字符。 |
| customForgotMyPasswordText | String | 用于替换登录窗体上的默认“忘记我的密码”超链接文本的字符串。 此文本必须采用 Unicode 格式，且不超过 256 个字符。 |
| customPrivacyAndCookiesText | String | 用于替换页脚中的默认“隐私和 Cookie”超链接文本的字符串。 此文本必须采用 Unicode 格式，且不超过 256 个字符。 |
| customPrivacyAndCookiesUrl | String | 一个自定义 URL，用于替换页脚中“隐私和 Cookie”超链接的默认 URL。 此 URL 必须采用 ASCII 格式，否则非 ASCII 字符必须进行 URL 编码，且不超过 128 个字符。 |
| customTermsOfUseText | String | 用于替换页脚中的默认“使用条款”超链接文本的字符串。 此文本必须采用 Unicode 格式，且不超过 256 个字符。 |
| customTermsOfUseUrl | String | 用于替换页脚中“使用条款”超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，否则必须对非 ASCII 字符进行 URL 编码，且不能超过 128 个字符。 |
| favicon | Stream | 用于替换 Azure AD 租户上的默认 Microsoft 产品 favicon 的自定义图标 (favicon) 。 |
| headerBackgroundColor | String | 用于自定义标头颜色的 RGB 颜色。 |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | 表示可以在租户的登录页上隐藏的各种文本。 可以更新所有属性。 |
| signInPageText | String | 登录框底部显示的文本。 使用此功能可以传达其他信息，例如，将电话号码传达给您的技术支持人员或法律声明。 此文本必须采用 Unicode 格式，且不超过 1024 个字符。 |
| squareLogo | Stream | 在 OOBE) 和 Windows Autopilot 启用部署时，Windows 10现 (体验中显示的公司徽标的平方版本。 允许的类型是 PNG 或 JPEG，大小不超过 240 x 240 像素，大小不超过 10 KB。 建议使用不填充徽标的透明图像。|
| usernameHintText | String | 一个字符串，显示为登录屏幕上用户名文本框中的提示。 此文本必须是 Unicode，没有链接或代码，不能超过 64 个字符。 |

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

以下请求更新了本地化的 `fr-FR` 横幅徽标。

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization6-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocalization6-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-a-default-branding-value-with-a-blank-string"></a>示例 3：使用空白字符串替代默认品牌值

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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization7-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocalization7-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

在请求之后，本地化的 **usernameHintText** `fr-FR` 将为空，而不是从默认品牌对象继承值。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
