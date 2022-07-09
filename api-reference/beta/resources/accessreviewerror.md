---
title: accessReviewError 资源类型
description: 表示访问评审实例生命周期内发生的错误。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7e0b773bd8b1393b160cb666db4d5f19d9501a54
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697923"
---
# <a name="accessreviewerror-resource-type"></a>accessReviewError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示访问评审实例生命周期中发生的错误。 此资源是只读的。

继承自 [genericError](../resources/genericerror.md)。

## <a name="properties"></a>属性
| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| code  |字符串  | 表示错误类型。 继承自 genericError。 只读。 |
| message |String | 表示错误详细信息。 继承自 genericError。 只读。|

## <a name="relationships"></a>关系
无。


## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewError"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
