---
title: integerRange 资源类型
description: 表示由两个 Int64 边界描述的非独占整数范围。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: b869d99fc4fef8b6804a3559ddd21e7d661ea32b
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899433"
---
# <a name="integerrange-resource-type"></a>integerRange 资源类型

命名空间：microsoft.graph

表示由两个 Int64 边界描述的非独占整数范围。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|start|Int64|整数范围的非独占下限。|
|end|Int64|整数范围的非独占上限。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.integerRange"
}
-->
```json
{
    "start": 12345,
    "end": 12345
}
```
