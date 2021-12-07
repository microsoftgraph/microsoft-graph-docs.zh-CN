---
title: callParticipantInfo 资源类型
description: 表示呼叫参与者的详细信息。
author: RamjotSingh
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 95b0e796092f2e9f2ddf480b586d9e50eead0380
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322407"
---
# <a name="callparticipantinfo-resource-type"></a>callParticipantInfo 资源类型

命名空间：microsoft.graph

表示呼叫参与者的详细信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|参与者|[identitySet](../resources/identityset.md)|呼叫参与者的标识。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callParticipantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callParticipantInfo",
  "participant": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

