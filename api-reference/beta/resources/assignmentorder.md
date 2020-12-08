---
title: assignmentOrder 资源类型
description: 用于定义在用户流中收集的属性的顺序。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 41b75e1adf5459279b5675278a8f00a82110b457
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581288"
---
# <a name="assignmentorder-resource-type"></a>assignmentOrder 资源类型

命名空间：microsoft.graph

用于定义在用户流中收集的属性的顺序。 这将确定当用户通过用户流注册时，如何显示属性集合页。

## <a name="properties"></a>属性

|属性|类型|Description|
|:---|:---|:---|
|顺序|字符串集合|提供的 identityUserFlowAttribute Id 的列表，用于确定应在用户流中收集属性的顺序。|

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
