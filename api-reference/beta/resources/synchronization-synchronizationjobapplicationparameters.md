---
title: synchronizationJobApplicationParameters 资源类型
description: 表示要设置的对象以及在按需预配时执行的规则。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0f0b7cae5a3ce9c49ea64b603390ea65831144b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007153"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>synchronizationJobApplicationParameters 资源类型

命名空间：microsoft.graph

表示将设置的对象和执行的同步规则。 资源主要用于按需预配。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ruleId|String|要应用的 synchronizationRule 的标识符;对于具有单个 synchronizationRule 的 synchronizationJob 是可选的。|
|聚焦|[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)集合|要应用 synchronizationJob 的一个或多个对象的标识符。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobApplicationParameters",
  "ruleId": "String",
  "subjects": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```
