---
title: serviceAnnouncement 资源类型
description: 服务通信资源的顶级容器
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: 761594fd25e31fe7b1edd009db234a491ff5d11e
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266728"
---
# <a name="serviceannouncement-resource-type"></a>serviceAnnouncement 资源类型

命名空间：microsoft.graph

服务通信资源的顶级容器。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 healthOverviews](../api/serviceannouncement-list-healthoverviews.md)|[serviceHealth](../resources/servicehealth.md) 集合|从 healthOverviews 导航属性获取 serviceHealth 资源。|
|[列出问题](../api/serviceannouncement-list-issues.md)|[serviceHealthIssue](../resources/servicehealthissue.md) 集合|从 issues 导航属性获取 serviceHealthIssue 资源。|
|[列出邮件](../api/serviceannouncement-list-messages.md)|[serviceUpdateMessage](../resources/serviceupdatemessage.md) 集合|从 messages 导航属性获取 serviceUpdateMessage 资源。|

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
|属性|类型|说明|
|-|-|-|
|messages|collection ([serviceUpdateMessage) ](serviceupdatemessage.md)|租户的服务消息集合。 此属性是包含的导航属性，可为空且可读。|
|healthOverviews|collection ([serviceHealth](servicehealth.md)) |租户的服务运行状况信息的集合。 此属性是包含的导航属性，可为空且可读。|
|问题|collection ([serviceHealthIssue) ](servicehealthissue.md)|租户的服务问题集合。 此属性是包含的导航属性，可为空且可读。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceAnnouncement",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceAnnouncement"
}
```