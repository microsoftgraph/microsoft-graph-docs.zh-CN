---
title: organizationalBrandingLocalization 资源类型
description: 包含组织品牌本地化的详细信息。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b01a52bd81c5b1cbbaf8611ab0efd96c75f229b5
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62804624"
---
# <a name="organizationalbrandinglocalization-resource-type"></a>organizationalBrandingLocalization 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

支持管理特定语言品牌的资源。 虽然你无法更改原始配置的语言，但此资源允许你为另一种语言创建新配置。

继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 organizationalBrandingLocalizations](../api/organizationalbranding-list-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 集合|获取 [organizationalBrandingLocalization 对象](../resources/organizationalbrandinglocalization.md) 及其属性的列表。|
|[创建 organizationalBrandingLocalization](../api/organizationalbranding-post-localizations.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|创建新的 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象。|
|[Get organizationalBrandingLocalization](../api/organizationalbrandinglocalization-get.md)|[organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md)|读取 [organizationalBrandingLocalization 对象的属性和](../resources/organizationalbrandinglocalization.md) 关系。|
|[更新 organizationalBrandingLocalization](../api/organizationalbrandinglocalization-update.md)| 无 |更新 [organizationalBrandingLocalization 对象](../resources/organizationalbrandinglocalization.md) 的属性。|
|[删除 organizationalBrandingLocalization](../api/organizationalbrandinglocalization-delete.md)|无|删除 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象。|

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| backgroundColor | 字符串 | 在低带宽连接中显示的颜色，用于表示背景图像。 我们建议你使用横幅徽标的主要颜色或你的组织颜色。 以十六进制格式指定此参数，例如，white 为 `#FFFFFF`。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| backgroundImage | Stream | 显示为登录页背景的图像。 允许的类型是 PNG 或 JPEG，不小于 300 KB 且不超过 1920 × 1080 像素。 较小的图像将降低带宽要求，并加快页面加载速度。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| backgroundImageRelativeUrl | 字符串 | **backgroundImage** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN。 只读。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| bannerLogo | Stream | 显示在登录页上的公司徽标的横幅版本。 允许的类型是 PNG 或 JPEG 不超过 36 × 245 像素。 我们建议使用透明图像，徽标周围没有填充。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| bannerLogoRelativeUrl | 字符串 | **bannerLogo** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN 提供的只读版本。 只读。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| cdnList | 字符串集合 | 提供当前资源资产的所有可用CDN提供程序的基本 URL 列表。 多个CDN提供程序同时用于读取请求的高可用性。 只读。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customAccountResetCredentialsUrl | 字符串 | 用于重置帐户凭据的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customCannotAccessYourAccountText | 字符串 | 一个字符串，用于替换默认字符串"无法访问你的帐户？" 登录页上 (SSPR) 超链接文本的自助服务密码重置。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customCannotAccessYourAccountUrl | 字符串 | 用于替换 SSPR 中自助服务密码重置的默认 URL 的自定义 URL (SSPR) "无法访问您的帐户？" 超链接。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 <br/><br/>**请勿使用。** 请 **改为使用 customAccountResetCredentialsUrl** 。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customForgotMyPasswordText | 字符串 | 一个字符串，用于替换登录表单上的默认"忘记密码"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customPrivacyAndCookiesText | 字符串 | 一个字符串，用于替换页脚中的默认"隐私和 Cookie"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customPrivacyAndCookiesUrl | 字符串 | 用于替换页脚中"隐私和 Cookie"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customResetItNowText | 字符串 | 一个字符串，用于替换登录表单上默认的"立即重置"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 <br/><br/>**请勿使用：** 目前不支持自定义"现在重置它"超链接文本。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customTermsOfUseText | 字符串 | 一个字符串，用于替换页脚中的默认"使用条款"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| customTermsOfUseUrl | 字符串 | 用于替换页脚中"使用条款"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，并且不得超过 128 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| favicon | Stream | 自定义图标 (替换) 租户上的默认 Microsoft 产品Azure AD图标。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| faviconRelativeUrl | 字符串 | 上述 favicon 的相对 URL，该 url 与 **cdnList** CDN基 URL 结合使用，以提供由 CDN。 只读。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| headerBackgroundColor | 字符串 | 要应用以自定义页眉颜色的 RGB 颜色。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| id | 字符串 | 表示使用区域性名称指定的区域设置的标识符。 区域性名称遵循 RFC 1766 标准，格式为"languagecode2-country/regioncode2"，其中"languagecode2"是派生自 ISO 639-1 的大写两字母代码，而"country/regioncode2"是派生自 ISO 3166 的大写两字母代码。 例如，美国英语为 `en-US`。 默认 /branding 的 **ID** 始终为 String 类型或 `0` `default`。 只读。 <br/><br/>**注意：** 目前不支持单个区域设置的多个品牌。 |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](loginPageTextVisibilitySettings.md) | 表示可在租户的登录页上隐藏的各种文本。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| signInPageText | 字符串 | 显示在登录框底部的文本。 使用它来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须采用 Unicode 格式，且不得超过 1024 个字符。 |
| squareLogo | Stream | 显示在 Windows 10 OOBE (OOBE) 和启用 Windows Autopilot 进行部署的现成功能中的公司徽标的正方形版本。 允许的类型是 PNG 或 JPEG，其大小不超过 240 x 240 像素且大小不超过 10 KB。 我们建议使用透明图像，徽标周围没有填充。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。|
| squareLogoRelativeUrl | 字符串 | **squareLogo** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN。 只读。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |
| usernameHintText | 字符串 | 一个字符串，在登录屏幕的用户名文本框中作为提示显示。 此文本必须是不带链接或代码的 Unicode，并且不能超过 64 个字符。 继承自 [organizationalBrandingProperties](organizationalbrandingproperties.md)。 |

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization",
  "baseType": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingLocalization",
  "id": "String (identifier)",
  "backgroundColor": "String",
  "backgroundImage": "Stream",
  "backgroundImageRelativeUrl": "String",
  "bannerLogo": "Stream",
  "bannerLogoRelativeUrl": "String",
  "cdnList": [
    "String"
  ],
  "signInPageText": "String",
  "squareLogo": "Stream",
  "squareLogoRelativeUrl": "String",
  "usernameHintText": "String",
  "customAccountResetCredentialsUrl": "String",
  "customCannotAccessYourAccountText": "String",
  "customCannotAccessYourAccountUrl": "String",
  "customForgotMyPasswordText": "String",
  "customPrivacyAndCookiesText": "String",
  "customPrivacyAndCookiesUrl": "String",
  "customResetItNowText": "String",
  "customTermsOfUseText": "String",
  "customTermsOfUseUrl": "String",
  "favicon": "Stream",
  "faviconRelativeUrl": "String",
  "headerBackgroundColor": "String",
  "loginPageTextVisibilitySettings": {
    "@odata.type": "microsoft.graph.loginPageTextVisibilitySettings"
  }
}
```