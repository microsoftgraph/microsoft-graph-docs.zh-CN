---
title: integerRange 资源类型
description: 表示由两个 Int64 边界描述的整数的包含范围。
author: nilakhan
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 6af69a7184a88d8540b45b35a58875b5d2934712fa0915bb0d1e59df2623697d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146858"
---
# <a name="integerrange-resource-type"></a>integerRange 资源类型

命名空间：microsoft.graph

表示由两个 Int64 边界描述的整数的包含范围。

## <a name="properties"></a>属性
| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|start|Int64|整数范围的包含边界下限。|
|end|Int64|整数范围的包含上限。|

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