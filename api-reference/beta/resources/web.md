---
title: web 资源类型
description: 指定 web 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: 26efe59eda739597e7193fa1ff79443f3d64b5a7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890200"
---
# <a name="web-resource-type"></a>web 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

指定 web 应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | Description |
|:---------|:-----|:------------|
|implicitGrantSettings|[implicitGrantSettings](implicitgrantsettings.md)| 指定此 web 应用程序是否可以请求令牌使用 OAuth 2.0 隐式流。|
|logoutUrl|字符串| 指定将由 Microsoft 的授权服务的用户使用[前信道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议的注销 URL。 |
|oauth2AllowImplicitFlow|布尔| 已弃用。 请勿使用。 | 
|redirectUris|String 集合| 指定用于登录，用户令牌发送到的 Url 或 Uri 的 OAuth 2.0 授权代码和访问令牌发送到的重定向。 |

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.web"
}-->

```json
{
  "implicitGrantSettings": {"@odata.type": "microsoft.graph.implicitGrantSettings"},
  "logoutUrl": "String",
  "oauth2AllowImplicitFlow": false,
  "redirectUris": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
