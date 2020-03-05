---
title: onlineMeetingInfo 资源类型
description: 关于与会者如何加入联机会议的详细信息。
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac6c42f28ed1f2adccd54fcd3bd6667f4113b7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522247"
---
# <a name="onlinemeetinginfo-resource-type"></a>onlineMeetingInfo 资源类型

命名空间： microsoft. graph

关于与会者如何加入联机会议的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|conferenceId|String| 会议的 ID。|
|joinUrl|String| 启动联机会议的外部链接。 这是客户端将启动到浏览器并将重定向用户加入会议的 URL。|
|phones|[phone](phone.md) collection| 与此会议关联的所有电话号码。|
|quickDial|String| 此调用的预格式化的 quickdial。|
|tollFreeNumbers|String 集合| 可用于加入会议的免费电话号码。|
|tollNumber|String| 可用于加入会议的收费号码。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->s
