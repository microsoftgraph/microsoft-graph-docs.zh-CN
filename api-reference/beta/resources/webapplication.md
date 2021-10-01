---
title: webApplication 资源类型
description: 指定 Web 应用程序的设置。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f4f6ec9d65dd6d30b54b030651178484392fba06
ms.sourcegitcommit: 0ec845f93eaa140ad833ba163c76c5308197a92f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2021
ms.locfileid: "60068542"
---
# <a name="webapplication-resource-type"></a>webApplication 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定 Web 应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------|:-----|:------------|
| homePageUrl | String | 应用程序的主页或登录页面。 |
| implicitGrantSettings | [implicitGrantSettings](implicitgrantsettings.md)| 指定此 Web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。 |
| logoutUrl | String | 指定 Microsoft 授权服务使用[正向通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[反向通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户时所使用的 URL。 |
| redirectUris | String collection | 指定用于登录的用户令牌的 URL，或发送 OAuth 2.0 授权代码和访问令牌的重定向 URI。 |
|redirectUriSettings| [redirectUriSettings](redirecturisettings.md) 集合 | 指定发送用户令牌用于登录的 URL 的索引。 这仅适用于使用 SAML 的应用程序。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webApplication"
}-->

```json
{
  "homePageUrl": "String",
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "redirectUris": ["String"],
  "redirectUriSettings": [
    {
      "@odata.type": "microsoft.graph.redirectUriSettings"
    }
  ],
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "webApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


