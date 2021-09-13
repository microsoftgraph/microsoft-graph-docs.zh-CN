---
title: synchronizationJobApplicationParameters 资源类型
description: 表示要设置的对象以及按需设置期间执行的规则。
author: ArvindHarinder1
ms.localizationpriority: medium
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: aeaae3419307787c019402d5b8ddf8268f1f9605
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59090956"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a>synchronizationJobApplicationParameters 资源类型

命名空间：microsoft.graph

表示将设置的对象和执行的同步规则。 资源主要用于按需预配。 

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|ruleId|String|要应用的 synchronizationRule 的标识符。|
|主题|[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) 集合|要应用 synchronizationJob 的一个或多个对象的标识符。|

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


