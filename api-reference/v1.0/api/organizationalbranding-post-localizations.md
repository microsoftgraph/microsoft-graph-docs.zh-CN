---
title: 创建 organizationalBrandingLocalization
description: 创建新的 organizationalBrandingLocalization 对象。
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 03c2112f78f011a2deb67248e7e62642f4caa15d
ms.sourcegitcommit: 7ce66321abb6a2cdca8685d3ce0a004c376ae33b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777989"
---
# <a name="create-organizationalbrandinglocalization"></a>创建 organizationalBrandingLocalization
命名空间：microsoft.graph

创建新的 [organizationalBrandingLocalization](../resources/organizationalBrandingLocalization.md) 对象。 这将创建本地化品牌，同时创建默认品牌（如果不存在）。

默认品牌仅创建一次。 当未为用户的浏览器语言配置本地化品牌时，将加载它。 若要检索默认品牌，请参阅获取 [品牌](organizationalbranding-get.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Organization.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
如果还没有本地化品牌，此请求将创建新的本地化品牌和默认品牌。 
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/branding/localizations
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

下表显示创建 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象时所需的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| id | String | 表示 ISO 639-1 标准中指定的区域设置（例如，英语）的标识符 `en-US` 。 无法将 **id** 的值设置为 String 类型或 来创建默认 `0` 品牌 `default` 。  <br/><br/>**注意：** 目前不支持单个区域设置的多个品牌。 |

## <a name="response"></a>响应

如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) 对象。

## <a name="examples"></a>示例

以下示例为法语和本地化创建 () `fr-FR` 本地化。 String 类型的任何未指定属性都继承自默认品牌对象中的值。 例如，如果默认品牌对象中的 signInPageText 为 ，则在此请求中创建的品牌的 `null` signInPageText `fr-FR` 也将为 `null` 。 若要替代 `null` 不带任何文本的值，请使用仅包含空格的字符串。

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandinglocalization"
}-->
```http
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr-FR",
    "signInPageText": " "
}
```


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')/branding/localizations/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/directoryObjects/$/Microsoft.DirectoryServices.Organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')//localizations/fr-FR",
    "id": "fr-FR",
    "backgroundColor": "",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": null,
    "cdnList": [],
    "signInPageText": " ",
    "squareLogoRelativeUrl": null,
    "usernameHintText": ""
}
```