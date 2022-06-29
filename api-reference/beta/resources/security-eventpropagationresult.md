---
title: eventPropagationResult 资源类型
description: 表示所创建事件的成功状态以及有关作用域内位置的其他信息。
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: f8822b44020b2e76a41372b93f8bb71ee5f8bafe
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447600"
---
# <a name="eventpropagationresult-resource-type"></a>eventPropagationResult 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示保留事件创建请求的状态以及有关作用域内位置的其他信息。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|状态|microsoft.graph.security.eventPropagationStatus|指示事件创建请求的状态。 可能的值包括 `none`、`inProcessing`、`failed`、`success`。|
|statusInformation|String|有关事件创建请求状态的其他信息。|
|serviceName|String|与事件关联的工作负荷的名称。|
|位置|String|与事件关联的工作负荷中特定位置的名称。|


## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.eventPropagationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.eventPropagationResult",
  "workload": "String",
  "location": "String",
  "status": "String",
  "statusInformation": "String"
}
```


