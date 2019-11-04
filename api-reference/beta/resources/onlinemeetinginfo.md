---
title: onlineMeetingInfo 资源类型
description: 用于联机加入会议的与会者的详细信息。
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ed8543be8b1d22c797d0033dcd0d41ba6308888
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939388"
---
# <a name="onlinemeetinginfo-resource-type"></a>onlineMeetingInfo 资源类型

用于联机加入会议的与会者的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|conferenceId|字符串| 会议的 ID。|
|joinUrl|字符串| 启动联机会议的外部链接。 这是客户端将启动到浏览器并将重定向用户加入会议的 URL。|
|phones|[phone](phone.md) collection| 与此会议关联的所有电话号码。|
|quickDial|字符串| 此调用的预格式化的 quickdial。|
|tollFreeNumbers|String collection| 可用于加入会议的免费电话号码。|
|tollNumber|字符串| 可用于加入会议的收费号码。|

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
