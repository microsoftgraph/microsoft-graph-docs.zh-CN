---
title: onPremisesPublishing 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508179"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|customDomainCertificate|String|当正在使用中的自定义域名与应用程序关联的证书的详细信息。 为空时使用的默认域。|
|externalAuthenticationType|String|详细预身份验证设置的应用程序可能的值为： `passthru`， `aadPreAuthentication`。|
|externalUrl|String|应用程序的已发布外部 url。 例如：  |
|internalUrl|String|应用程序的内部 url。 例如： |
|isOnPremPublishingEnabled|Boolean|指示是否或不当前正在发布应用程序。|
|applicationServerTimeout|String|连接器将等待响应之前关闭该连接的后端应用程序持续时间。 可取值为：`default`、`long`。 使用`long`如果您的服务器所需超过 60 75 秒来响应请求。 此外尝试`long`如果您不能访问应用程序，并且错误状态为"后端超时"。|
|isTranslateHostHeaderEnabled|Boolean|指示应用程序应翻译响应头中的 url。 这包括设置正确的站点的 cookie。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
