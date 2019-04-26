---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 8531a68ad56dad0f44ef8cd55e9fabeff47a6c2e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341786"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customDomainCertificate|String|使用自定义域时与应用程序关联的证书的详细信息。 使用默认域时为 Null。|
|externalAuthenticationType|String|详细说明应用程序的预身份验证设置可能的值为`passthru`: `aadPreAuthentication`、。|
|externalUrl|String|应用程序的已发布外部 url。 例如https://intranet-contoso.msappproxy.net/  |
|internalUrl|String|应用程序的内部 url。 例如https://intranet/ |
|isOnPremPublishingEnabled|Boolean|指示应用程序当前是否正在发布。|
|applicationServerTimeout|String|在关闭连接之前, 连接器将等待后端应用程序响应的持续时间。 可能的值`default`为`long`。 如果`long`服务器要响应请求的时间超过60-75 秒, 请使用。 此外, `long`如果您无法访问应用程序, 并且错误状态为 "后端超时", 也会尝试。|
|isTranslateHostHeaderEnabled|Boolean|指示应用程序是否应转换响应标头中的 url。 这包括为 cookie 设置正确的网站。|

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
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
