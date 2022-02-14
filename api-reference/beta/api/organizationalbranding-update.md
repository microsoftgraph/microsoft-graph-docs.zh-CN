---
title: Update organizationalBranding
description: 更新 organizationalBranding 对象的属性。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 073422bb2d6d831c8640de781aa4b6093b5025ba
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804484"
---
# <a name="update-organizationalbranding"></a>Update organizationalBranding
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [organizationalBranding](../resources/organizationalbranding.md) 资源指定的默认品牌对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|
|Accept-Language|有效的 ISO 639-1 区域设置。 必需。|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| backgroundColor | 字符串 | 在低带宽连接中显示的颜色，用于表示背景图像。 我们建议你使用横幅徽标的主要颜色或你的组织颜色。 以十六进制格式指定此参数，例如，white 为 `#FFFFFF`。 |
| backgroundImage | Stream | 显示为登录页背景的图像。 允许的类型是 PNG 或 JPEG，不小于 300 KB 且不超过 1920 × 1080 像素。 较小的图像将降低带宽要求，并加快页面加载速度。 |
| bannerLogo | Stream | 显示在登录页上的公司徽标的横幅版本。 允许的类型是 PNG 或 JPEG 不超过 36 × 245 像素。 我们建议使用透明图像，徽标周围没有填充。 |
| customAccountResetCredentialsUrl | 字符串 | 用于重置帐户凭据的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 |
| customCannotAccessYourAccountText | 字符串 | 一个字符串，用于替换默认字符串"无法访问你的帐户？" 自助密码重置 (SSPR) 登录页面上的超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customForgotMyPasswordText | 字符串 | 一个字符串，用于替换登录表单上的默认"忘记密码"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customPrivacyAndCookiesText | 字符串 | 一个字符串，用于替换页脚中的默认"隐私和 Cookie"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customPrivacyAndCookiesUrl | 字符串 | 用于替换页脚中"隐私和 Cookie"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 |
| customTermsOfUseText | 字符串 | 一个字符串，用于替换页脚中的默认"使用条款"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customTermsOfUseUrl | 字符串 | 用于替换页脚中"使用条款"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，并且不得超过 128 个字符。 |
| favicon | Stream | 自定义图标 (替换) 租户上的默认 Microsoft 产品Azure AD图标。 |
| headerBackgroundColor | 字符串 | 要应用以自定义页眉颜色的 RGB 颜色。 |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | 表示可在租户的登录页上隐藏的各种文本。 所有属性都可以更新。 |
| signInPageText | 字符串 | 显示在登录框底部的文本。 使用它来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须采用 Unicode 格式，且不得超过 1024 个字符。 |
| squareLogo | Stream | 显示在 Windows 10 OOBE (OOBE) 和启用 Windows Autopilot 进行部署的现成功能中的公司徽标的正方形版本。 允许的类型是 PNG 或 JPEG，其大小不超过 240 x 240 像素且大小不超过 10 KB。 我们建议使用透明图像，徽标周围没有填充。|
| usernameHintText | 字符串 | 一个字符串，在登录屏幕的用户名文本框中作为提示显示。 此文本必须是不带链接或代码的 Unicode，并且不能超过 64 个字符。 |

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="example-1-update-the-default-branding"></a>示例 1：更新默认品牌

#### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_1"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding
Content-Type: application/json
Accept-Language: 0

{
    "signInPageText":"Default",
    "usernameHintText":"DefaultHint"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocaliation-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocaliation-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocaliation-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocaliation-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocaliation-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocaliation-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-bannerlogo-for-the-default-branding"></a>示例 2：更新默认品牌打造的 bannerLogo

以下请求更新默认品牌打造的横幅徽标。

#### <a name="request"></a>请求

下面展示了示例请求。



<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocaliation_2"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/bannerLogo
Content-Type: image/jpeg

<Image>
```



#### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
