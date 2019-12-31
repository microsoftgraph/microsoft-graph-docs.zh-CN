---
title: onlineMeetingInfo 资源类型
description: 关于与会者如何加入联机会议的详细信息。
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 52bfe4fd46443c826838153cc2a40ea57712182b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913154"
---
# <a name="onlinemeetinginfo-resource-type"></a>onlineMeetingInfo 资源类型

关于与会者如何加入联机会议的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|conferenceId|String| 会议的 ID。|
|joinUrl|String| 启动联机会议的外部链接。 这是客户端将启动到浏览器并将重定向用户加入会议的 URL。|
|phones|[phone](phone.md) collection| 与此会议关联的所有电话号码。|
|quickDial|String| 此调用的预格式化的 quickdial。|
|tollFreeNumbers|String collection| 可用于加入会议的免费电话号码。|
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
