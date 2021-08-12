---
title: serviceUserAgent 资源类型
description: serviceUserAgent 类型
localization_priority: Normal
author: williamlooney
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bb8880b130c763599d75c5542725f1bb0fe850bad532693a62ee73ff25ffbfb3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54243628"
---
# <a name="serviceuseragent-resource-type"></a>serviceUserAgent 资源类型

命名空间：microsoft.graph.callRecords

表示呼叫中终结点的服务用户代理。 继承自 [userAgent](callrecords-useragent.md) 类型。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|applicationVersion|String|标识此终结点使用的应用程序软件的版本。|
|headerValue|String|此终结点报告的用户代理标头值。|
|role|microsoft.graph.callRecords.serviceRole|标识此终结点使用的服务的角色。 可能的值是 `unknown` `customBot` `skypeForBusinessMicrosoftTeamsGateway` ：、、、、、、、、、、 `skypeForBusinessAudioVideoMcu` `skypeForBusinessApplicationSharingMcu` `skypeForBusinessCallQueues` `skypeForBusinessAutoAttendant` `mediationServer` `mediationServerCloudConnectorEdition` `exchangeUnifiedMessagingService` `mediaController` `conferencingAnnouncementService` `conferencingAttendant` `audioTeleconferencerController` `skypeForBusinessUnifiedCommunicationApplicationPlatform` `responseGroupServiceAnnouncementService` `gateway` `skypeTranslator` `skypeForBusinessAttendant` `responseGroupService` `voicemail` `unknownFutureValue` 。|

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
