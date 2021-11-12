---
title: printMargin 资源类型
description: 指定打印时使用的边距宽度。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 20ad208efdac2890a45dfbebdcf51ace8e49d061
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60924206"
---
# <a name="printmargin-resource-type"></a>printMargin 资源类型

命名空间：microsoft.graph

指定打印时使用的边距宽度。

## <a name="properties"></a>属性
|属性|类型|Description|
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

