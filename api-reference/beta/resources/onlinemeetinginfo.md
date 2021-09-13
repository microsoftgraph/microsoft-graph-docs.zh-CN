---
title: onlineMeetingInfo 资源类型
description: 关于与会者如何加入联机会议的详细信息。
ms.localizationpriority: medium
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 325840e11b93658abe3294edf339175bebe03daf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023225"
---
# <a name="onlinemeetinginfo-resource-type"></a>onlineMeetingInfo 资源类型

命名空间：microsoft.graph

关于与会者如何加入联机会议的详细信息。

## <a name="properties"></a>属性

| 属性     | 类型        | 描述 |
|:-------------|:------------|:------------|
|conferenceId|String| 会议的 ID。|
|joinUrl|String| 启动联机会议的外部链接。 这是一个 URL，客户端将启动到浏览器中，并重定向用户以加入会议。|
|phones|[phone](phone.md) collection| 与此会议关联的所有电话号码。|
|quickDial|String| 此调用的预先格式化的快速拨叫。|
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


