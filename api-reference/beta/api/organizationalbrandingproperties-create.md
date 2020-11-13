---
title: 创建 organizationalBrandingProperties
description: 创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: efb10cd5669022dda2afd385ea013ae110a97ea0
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031939"
---
# <a name="create-organizationalbrandingproperties"></a>创建 organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。 这将同时创建默认品牌打造和本地化品牌（可选）。 当本地化品牌集未配置为使用用户的浏览器语言时，将加载默认品牌。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

如果尚不存在使用 PUT 或 PATCH 的组织，则会为组织创建一个品牌。

如果已配置品牌，则 PUT 将覆盖所有现有值，而不管请求正文中的内容如何。 修补程序将仅 overite 请求正文中包含的值，并将不包含的值保持不变。

对/branding singleton 的 PUT/PATCH 忽略 **id** 属性。 如果未指定内容语言，则会创建默认品牌，它对应于的 **id** `und` 。 如果指定了 Content 语言，则会为该区域设置创建品牌。
<!-- { "blockType": "ignored" } -->

```http
PUT /organization/{id}/branding
PATCH /organization/{id}/branding
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用某些 OData 查询参数来帮助自定义响应。有关常规信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required.  |
| Content-Language  | 位置. 可选。  |

## <a name="request-body"></a>请求正文

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|backgroundColor|String|将在低带宽连接中的背景图像处显示的颜色。 建议在此处使用横幅徽标的主要颜色或您的组织颜色。 在十六进制 (中指定此项例如，白色为 #FFFFFF) 。|
|backgroundImage|Stream|显示为登录页的背景的图像。 .png 或 .jpg 不大于1920x1080 且小于300kb。 较小的图像将降低带宽要求并使页面加载更具性能。|
|bannerLogo|Stream|显示在登录页面上的公司徽标的标题版本。 .png 或 .jpg 不大于36x245px。 我们建议使用透明图像，而不在徽标周围进行填充。|
|signInPageText|String|出现在登录框底部的文本。 您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。 此文本必须是 Unicode，且不能超过1024个字符。|
|squareLogo|Stream|公司徽标的平方版本。 在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。 .png 或 .jpg 不大于240x240px，且大小不超过10kb。 我们建议使用透明图像，而不在徽标周围进行填充。|
|usernameHintText|String|在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。 此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。|

## <a name="response"></a>响应

如果成功，此方法 `201 Created` 在响应正文中返回响应代码和创建的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。

## <a name="examples"></a>示例

下面的示例为 en-us 创建了默认的品牌打造和本地化。

### <a name="request"></a>请求

下面展示了示例请求。
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

在这种情况下，将设置默认品牌化对象。 由于标头中的内容语言，即使在响应中未返回 en-us 品牌设置，也会对 en-us 的本地化品牌进行设置。 请注意，请求中的内容语言是可选的，如果不存在，将仅设置默认品牌。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
