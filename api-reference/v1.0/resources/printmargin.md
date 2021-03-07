---
title: printMargin 资源类型
description: 指定打印时使用的边距宽度。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 1680cc641da02f3339dcd75977c411d3255cf037
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517291"
---
# <a name="printmargin-resource-type"></a>printMargin 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

指定打印时使用的边距宽度。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|top|Int32|上边缘的边距（以密分表示）。|
|bottom|Int32|下边缘的边距（以密分表示）。|
|right|Int32|右边缘的边距（以密分表示）。|
|左边|Int32|距左边缘的边距（以密分表示）。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printMargin"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printMargin",
  "top": "Integer",
  "bottom": "Integer",
  "right": "Integer",
  "left": "Integer"
}
```

