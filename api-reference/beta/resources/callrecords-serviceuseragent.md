---
title: serviceUserAgent 资源类型
description: ServiceUserAgent 类型
localization_priority: Normal
author: stephenjust
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c8cfe517b127bcdf359c69ab600146593f5ef288
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394686"
---
# <a name="serviceuseragent-resource-type"></a>serviceUserAgent 资源类型

命名空间： callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示呼叫中终结点的服务用户代理。 继承自[userAgent](callrecords-useragent.md)类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|applicationVersion|String|标识此终结点使用的应用程序软件的版本。|
|headerValue|String|此终结点报告的用户代理标头值。|
|role|String|标识此终结点使用的服务的角色。 可取值为：`unknown`、`customBot`、`skypeForBusinessMicrosoftTeamsGateway`、`skypeForBusinessAudioVideoMcu`、`skypeForBusinessApplicationSharingMcu`、`skypeForBusinessCallQueues`、`skypeForBusinessAutoAttendant`、`mediationServer`、`mediationServerCloudConnectorEdition`、`exchangeUnifiedMessagingService`、`mediaController`、`conferencingAnnouncementService`、`conferencingAttendant`、`audioTeleconferencerController`、`skypeForBusinessUnifiedCommunicationApplicationPlatform`、`responseGroupServiceAnnouncementService`、`gateway`、`skypeTranslator`、`skypeForBusinessAttendant`、`responseGroupService`、`unknownFutureValue`。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callRecords.serviceUserAgent",
  "baseType": "microsoft.graph.callRecords.userAgent"
}-->

```json
{
  "applicationVersion": "String",
  "headerValue": "String",
  "role": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "serviceUserAgent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->