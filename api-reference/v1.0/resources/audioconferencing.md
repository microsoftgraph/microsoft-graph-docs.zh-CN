---
title: audioConferencing 资源类型
description: 表示联机会议的电话访问信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a656ac6e3e47daea1c35b5fb54d6354a93c27dc2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021727"
---
# <a name="audioconferencing-resource-type"></a>audioConferencing 资源类型

命名空间：microsoft.graph

表示 [onlineMeeting 的电话访问信息](onlinemeeting.md)。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明                                                                    |
|:--------------------|:--------|:-------------------------------------------------------------------------------|
| dialinUrl           | String  | 指向包含拨入信息且可从外部访问的网页的 URL。 |
| conferenceId        | String  | 联机会议的会议 ID。      |
| tollFreeNumber      | String  | 连接到音频会议提供商的免费电话号码。              |
| tollNumber          | String  | 连接到音频会议提供商的收费号码。                   |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.audioConferencing"
}-->
```json
{
  "dialinUrl": "String",
  "conferenceId": "String",
  "tollFreeNumber": "String",
  "tollNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "audioConferencing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

