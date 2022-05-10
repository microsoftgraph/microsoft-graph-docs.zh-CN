---
title: synchronizationJobApplicationParameters 资源类型
description: 表示要预配的对象和按需预配期间执行的规则。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 08dc3f6494a2c7e641f6ebfc81eb223aa990eb69
ms.sourcegitcommit: 39f94342cada98add34b0e5b260a7acffa6ff765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/10/2022
ms.locfileid: "65296449"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>synchronizationJobApplicationParameters 资源类型

命名空间：microsoft.graph

表示要预配的对象和执行的同步规则。 该资源主要用于按需预配。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ruleId|String|要应用的 [synchronizationRule](synchronization-synchronizationrule.md) 的标识符。 此规则 ID 在 [给定同步作业或模板的架构](../api/synchronization-synchronizationschema-get.md)中定义。 |
|科目|[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) 集合|要向其应用 synchronizationJob 的一个或多个对象的标识符。|

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


