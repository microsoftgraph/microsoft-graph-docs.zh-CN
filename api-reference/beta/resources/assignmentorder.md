---
title: assignmentOrder 资源类型
description: 用于定义在用户流中收集的属性的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7d7716cb4b13917aad33cd88afeb364a2891e3df
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761238"
---
# <a name="assignmentorder-resource-type"></a>assignmentOrder 资源类型

命名空间：microsoft.graph

用于定义在用户流中收集的属性的顺序。 THis 确定当用户通过用户流注册时属性集合页的显示方式。

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|order|字符串集合|提供的 identityUserFlowAttribute ID 列表，用于确定应在用户流中收集属性的顺序。|

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
