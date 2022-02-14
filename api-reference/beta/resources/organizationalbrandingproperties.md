---
title: organizationalBrandingProperties 资源类型
description: 包含组织品牌打造的详细信息。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 68831b6069df0ea94df36605ff9f1099dfd27feb
ms.sourcegitcommit: dbacb04ae7138ac3b109683e63a6ff27c166f421
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2022
ms.locfileid: "62805142"
---
# <a name="organizationalbrandingproperties-resource-type"></a>organizationalBrandingProperties 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

公开用于配置组织品牌的属性的抽象类型。

组织可以自定义Azure Active Directory (Azure AD) 登录页面，当用户登录到其组织的租户特定应用时，或当用户Azure AD用户名标识用户的租户时，会显示这些页面。 开发人员还可以阅读公司的品牌信息并自定义其应用体验，以使用其公司的品牌专门为登录用户定制它。

不能更改由 [organizationalBranding](organizationalbranding.md) 对象表示的原始配置语言。 但是，公司可以基于区域设置添加不同的品牌。 有关特定语言的品牌，请参阅 [organizationalBrandingLocalization](organizationalbrandinglocalization.md) 对象。

>[!NOTE]
>添加自定义品牌打造需要你拥有 Azure Active Directory (Azure AD) 高级版 1、高级版 2 或 Office 365 (应用Office 365许可证) 许可证。 有关许可和版本详细信息，请参阅注册[Azure AD Premium](/azure/active-directory/fundamentals/active-directory-get-started-premium)。
>
>Azure AD Premium全球实例为中国客户提供 Azure Active Directory。 Azure AD Premium由世纪银行在中国运营的 Azure 服务中当前不支持这些版本。 有关详细信息，请通过论坛Azure Active Directory[我们](https://feedback.azure.com/forums/169401-azure-active-directory/)。

## <a name="methods"></a>方法
无。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| backgroundColor | 字符串 | 在低带宽连接中显示的颜色，用于表示背景图像。 我们建议你使用横幅徽标的主要颜色或你的组织颜色。 以十六进制格式指定此参数，例如，white 为 `#FFFFFF`。 |
| backgroundImage | Stream | 显示为登录页背景的图像。 允许的类型是 PNG 或 JPEG，不小于 300 KB 且不超过 1920 × 1080 像素。 较小的图像将降低带宽要求，并加快页面加载速度。 |
| backgroundImageRelativeUrl | 字符串 | **backgroundImage** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN。 只读。 |
| bannerLogo | Stream | 显示在登录页上的公司徽标的横幅版本。 允许的类型是 PNG 或 JPEG 不超过 36 × 245 像素。 我们建议使用透明图像，徽标周围没有填充。 |
| bannerLogoRelativeUrl | 字符串 | **bannerLogo** 属性的相对 URL，与 **cdnList** 中的 CDN 基 URL 结合使用以提供由 CDN 提供的只读版本。 只读。 |
| cdnList | 字符串集合 | 提供当前资源资产的所有可用CDN提供程序的基 URL 列表。 多个CDN提供程序同时用于读取请求的高可用性。 只读。 |
| customAccountResetCredentialsUrl | 字符串 | 用于重置帐户凭据的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 |
| customCannotAccessYourAccountText | 字符串 | 一个字符串，用于替换默认字符串"无法访问你的帐户？" 自助密码重置 (SSPR) 登录页面上的超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customCannotAccessYourAccountUrl | 字符串 | 用于替换 SSPR 中自助服务密码重置的默认 URL 的自定义 URL (SSPR) "无法访问您的帐户？" 超链接。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 <br/><br/>**请勿使用。** 请 **改为使用 customAccountResetCredentialsUrl** 。 |
| customForgotMyPasswordText | 字符串 | 一个字符串，用于替换登录表单上的默认"忘记密码"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customPrivacyAndCookiesText | 字符串 | 一个字符串，用于替换页脚中的默认"隐私和 Cookie"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customPrivacyAndCookiesUrl | 字符串 | 用于替换页脚中"隐私和 Cookie"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，且不得超过 128 个字符。 |
| customResetItNowText | 字符串 | 一个字符串，用于替换登录表单上默认的"立即重置"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 <br/><br/>**请勿使用：** 目前不支持自定义"现在重置它"超链接文本。 |
| customTermsOfUseText | 字符串 | 一个字符串，用于替换页脚中的默认"使用条款"超链接文本。 此文本必须采用 Unicode 格式，且不得超过 256 个字符。 |
| customTermsOfUseUrl | 字符串 | 用于替换页脚中"使用条款"超链接的默认 URL 的自定义 URL。 此 URL 必须采用 ASCII 格式，或者非 ASCII 字符必须经过 URL 编码，并且不得超过 128 个字符。 |
| favicon | Stream | 自定义图标 (替换) 租户上的默认 Microsoft 产品Azure AD图标。 |
| faviconRelativeUrl | 字符串 | 上述 favicon 的相对 URL，该 url 与 **cdnList** CDN基 URL 结合使用，以提供由 CDN。 只读。 |
| headerBackgroundColor | 字符串 | 要应用以自定义页眉颜色的 RGB 颜色。 |
| id | 字符串 | 表示使用区域性名称指定的区域设置的标识符。 区域性名称遵循 RFC 1766 标准，格式为"languagecode2-country/regioncode2"，其中"languagecode2"是派生自 ISO 639-1 的大写两字母代码，而"country/regioncode2"是派生自 ISO 3166 的大写两字母代码。 例如，美国英语为 `en-US`。 默认 /branding 的 **ID** 始终为 String 类型或 `0` `default`。 只读。 <br/><br/>**注意：** 目前不支持单个区域设置的多个品牌。 |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](loginPageTextVisibilitySettings.md) | 表示可在租户的登录页上隐藏的各种文本。 |
| signInPageText | 字符串 | 显示在登录框底部的文本。 使用它来传达其他信息，例如电话号码到技术支持或法律声明。 此文本必须采用 Unicode 格式，且不得超过 1024 个字符。 |
| squareLogo | Stream | 显示在 Windows 10 OOBE (OOBE) 和启用 Windows Autopilot 进行部署的现成功能中的公司徽标的正方形版本。 允许的类型是 PNG 或 JPEG，其大小不超过 240 x 240 像素且大小不超过 10 KB。 我们建议使用透明图像，徽标周围没有填充。|
| squareLogoRelativeUrl | 字符串 | **squareLogo** 属性的相对 URL，与 **cdnList** CDN基 URL 结合使用以提供由 CDN。 只读。 |
| usernameHintText | 字符串 | 一个字符串，在登录屏幕的用户名文本框中作为提示显示。 此文本必须是不带链接或代码的 Unicode，并且不能超过 64 个字符。 |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.organizationalBrandingProperties",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizationalBrandingProperties",
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
