---
title: assignmentOrder 资源类型
description: 定义在用户流中收集的属性的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4c5faed250c07d5c4416c91a5452f1276c6b728e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882827"
---
# <a name="assignmentorder-resource-type"></a>assignmentOrder 资源类型

命名空间：microsoft.graph

用于定义在用户流中收集的属性的顺序。 顺序确定当用户使用用户流注册时属性集合页的显示方式。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|order|String 集合|identityUserFlowAttribute 对象标识符的列表，这些标识符确定应在用户流中收集属性的顺序。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentOrder"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.assignmentOrder",
  "order": [
    "String"
  ]
}
```
