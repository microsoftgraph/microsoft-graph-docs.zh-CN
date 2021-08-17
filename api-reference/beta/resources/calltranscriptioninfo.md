---
title: callTranscriptionInfo 资源类型
description: 表示单个 DTMF 事件。
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 27571ad09d6fe29c511b0efa59939dc65074235f9c0c2d4137251687068c47f0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54200794"
---
# <a name="calltranscriptioninfo-resource-type"></a>callTranscriptionInfo 资源类型

命名空间：microsoft.graph

表示单个 DTMF 事件。

## <a name="properties"></a>属性

| 属性       | 类型    | 说明|
|:---------------|:--------|:----------|
| state | String | 可取值为：`notStarted`、`active`、`inactive`。 |
| lastModifiedDateTime | 日期/时间 | 以 UTC 表示的修改时间状态。 |

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


