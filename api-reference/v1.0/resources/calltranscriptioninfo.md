---
title: callTranscriptionInfo 资源类型
description: 表示单个 DTMF 事件。
author: rzhang
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 92b95c3a6fde436ffbeca19620c3eed7f16d2297
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59067491"
---
# <a name="calltranscriptioninfo-resource-type"></a>callTranscriptionInfo 资源类型

命名空间：microsoft.graph

表示单个 DTMF 事件。

## <a name="properties"></a>属性

| 属性       | 类型    | 说明|
|:---------------|:--------|:----------|
| state | String | 可取值为：`notStarted`、`active`、`inactive`。 |
| lastModifiedDateTime | 日期时间 | 以 UTC 表示的修改时间状态。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.callTranscriptionInfo"
}-->
```json
{
  "state": "notStarted | active | inactive",
  "lastModifiedDateTime": "String (timestamp)"
}
```

