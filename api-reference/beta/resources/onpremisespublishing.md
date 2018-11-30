---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
ms.openlocfilehash: 8dba505347fc12d3c4a8521ebe32551d738dc4a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045356"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customDomainCertificate|字符串|当正在使用中的自定义域名与应用程序关联的证书的详细信息。 为空时使用的默认域。|
|externalAuthenticationType|字符串|详细预身份验证设置的应用程序可能的值为： `passthru`， `aadPreAuthentication`。|
|externalUrl|字符串|应用程序的已发布外部 url。 例如https://intranet-contoso.msappproxy.net/  |
|internalUrl|字符串|应用程序的内部 url。 例如https://intranet/ |
|isOnPremPublishingEnabled|布尔|指示是否或不当前正在发布应用程序。|
|applicationServerTimeout|字符串|连接器将等待响应之前关闭该连接的后端应用程序持续时间。 可能的值为`default`， `long`。 使用`long`如果您的服务器所需超过 60 75 秒来响应请求。 此外尝试`long`如果您不能访问应用程序，并且错误状态为"后端超时"。|
|isTranslateHostHeaderEnabled|布尔|指示应用程序应翻译响应头中的 url。 这包括设置正确的站点的 cookie。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
