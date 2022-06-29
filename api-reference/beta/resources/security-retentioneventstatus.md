---
title: retentionEventStatus 资源类型
description: 对于基于事件的保留，请在创建事件后提供事件传播到指定位置的状态。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: d21fabd92f19ac1be107568426e0c3e116e6a7ea
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447584"
---
# <a name="retentioneventstatus-resource-type"></a>retentionEventStatus 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

对于基于事件的保留，此属性在创建事件后向目标位置提供事件表示的状态。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|error|[microsoft.graph.publicError](../resources/publicerror.md)|如果状态不成功，则为错误。|
|状态|microsoft.graph.security.eventStatusType|分发的状态。 可能的值包括 `pending`、`error`、`success`、`notAvaliable`。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionEventStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionEventStatus",
  "error": {
    "@odata.type": "microsoft.graph.publicError"
  },
  "status": "String"
}
```

