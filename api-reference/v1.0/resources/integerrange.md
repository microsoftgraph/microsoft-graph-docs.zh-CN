---
title: integerRange 资源类型
description: 表示由两个 Int64 边界描述的整数的包含范围。
author: nilakhan
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 31661802fa198790e4d30f2da58ac11c86f19b6e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036478"
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
