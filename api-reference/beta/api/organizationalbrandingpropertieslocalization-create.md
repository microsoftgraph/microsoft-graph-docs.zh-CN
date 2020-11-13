---
title: 创建本地化的 organizationalBrandingProperties
description: 为特定区域设置创建组织品牌。
localization_priority: Normal
author: kexia
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 80849083686bab10626756197880ddfeade06c8b
ms.sourcegitcommit: 40b0e58312819b69567f35ab894ee0d2989837ab
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2020
ms.locfileid: "49031908"
---
# <a name="create-localized-organizationalbrandingproperties"></a>创建本地化的 organizationalBrandingProperties

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

为特定区域设置创建 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

发布到品牌/localizations 以创建新的本地化。 正文中指定的 id 是本地化的区域设置。 如果未指定 id，则内容语言标头的值（如果指定）将用作 id。如果没有指定 id，也未指定内容语言标头，则返回错误。
<!-- { "blockType": "ignored" } -->

```http
POST /organization/{id}/branding/localizations
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

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|backgroundColor|String|将在低带宽连接中的背景图像处显示的颜色。 建议在此处使用横幅徽标的主要颜色或您的组织颜色。 在十六进制 (中指定此项例如，白色为 #FFFFFF) 。|
|backgroundImage|Stream|显示为登录页的背景的图像。 .png 或 .jpg 不大于1920x1080 且小于300kb。 较小的图像将降低带宽要求并使页面加载更具性能。|
|bannerLogo|Stream|显示在登录页面上的公司徽标的标题版本。 .png 或 .jpg 不大于36x245px。 我们建议使用透明图像，而不在徽标周围进行填充。|
|signInPageText|String|出现在登录框底部的文本。 您可以使用它将其他信息（如电话号码）传递给技术支持或法律声明。 此文本必须是 Unicode，且不能超过1024个字符。|
|squareLogo|Stream|公司徽标的平方版本。 在 Windows 10 现成 (OOBE) 体验以及启用 Windows Autopilot 进行部署时，都会出现此对话框。 .png 或 .jpg 不大于240x240px，且大小不超过10kb。 我们建议使用透明图像，而不在徽标周围进行填充。|
|usernameHintText|String|在 "登录" 屏幕上的 "用户名" textbox 中显示为提示的字符串。 此文本必须是 Unicode，不含链接或代码，并且不能超过64个字符。|
|id|String|创建品牌的区域设置|

## <a name="response"></a>响应

如果成功，此方法 `201 CREATED` 在响应正文中返回响应代码和创建的 [organizationalBrandingProperties](../resources/organizationalbrandingproperties.md) 对象。

## <a name="examples"></a>示例

下面的示例创建了法语 (fr) 的品牌打造本地化。

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_organizationalbrandingproperties"
}-->

```http
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr"
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

{
    "backgroundColor":"#00000F",
    "backgroundImage@odata.mediaContentType":"image/*",
    "backgroundImage@odata.mediaReadLink": null,
    "backgroundImage@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/backgroundImage",
    "bannerLogo@odata.mediaContentType":"image/*",
    "bannerLogo@odata.mediaReadLink": null,
    "bannerLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/bannerLogo",
    "id": "fr",
    "squareLogo@odata.mediaContentType":"image/*",
    "squareLogo@odata.mediaReadLink": null,
    "squareLogo@odata.mediaEditLink": "https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr/squareLogo"
}
```
**MediaEditLink** 指定本地化的媒体的写入位置。 MediaReadLink 为 null，因为没有为本地化设置媒体。

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get organizationalBrandingProperties",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
