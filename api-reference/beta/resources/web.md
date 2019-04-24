---
title: web 资源类型
description: 指定 Web 应用程序的设置。
localization_priority: Normal
ms.openlocfilehash: 7e03977481f0c021b7d67ec44fd4db275642cdf8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453948"
---
# <a name="web-resource-type"></a>web 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定 Web 应用程序的设置。

## <a name="properties"></a>属性

| 属性 | 类型 | 描述 |
|:---------|:-----|:------------|
|implicitGrantSettings|[implicitGrantSettings](implicitgrantsettings.md)| 指定此 web 应用程序是否可以使用 OAuth 2.0 隐式流请求令牌。|
|logoutUrl|字符串| 指定将由 Microsoft 的授权服务用来使用[前通道](https://openid.net/specs/openid-connect-frontchannel-1_0.html)、[后通道](https://openid.net/specs/openid-connect-backchannel-1_0.html)或 SAML 注销协议注销用户的 URL。 |
|oauth2AllowImplicitFlow|Boolean| 已弃用。 请勿使用。 | 
|redirectUris|String collection| 指定向其发送用户令牌以进行登录的 url, 或向其发送 OAuth 2.0 授权代码和访问令牌的重定向 uri。 |

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
<!--
{
  "type": "#page.annotation",
  "description": "web resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/web.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
