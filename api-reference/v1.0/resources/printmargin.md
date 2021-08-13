---
title: printMargin 资源类型
description: 指定打印时使用的边距宽度。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d15b488985bbf1c51f03a0c030fab16fdf3d25cbd8c8b53b29368e4f0af2d151
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196563"
---
# <a name="printmargin-resource-type"></a>printMargin 资源类型

命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

指定打印时使用的边距宽度。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|top|Int32|上边缘的边距（以边距表示）。|
|bottom|Int32|下边缘的边距（以最低值表示）。|
|right|Int32|距右边缘的边距（以百分之二十表示）。|
|左边|Int32|距左边缘的边距（以百分之二十表示）。|

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

