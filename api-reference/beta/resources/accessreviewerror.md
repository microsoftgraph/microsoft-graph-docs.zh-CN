---
title: accessReviewError 资源类型
description: 表示在访问评审实例生命周期内发生的错误。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: dc0fe94daaba28bf92b20cb986760b0d3eb0901b
ms.sourcegitcommit: a598c09b73e4e43eea5f4aaefea7ffe062e15c39
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/22/2021
ms.locfileid: "53534251"
---
# <a name="accessreviewerror-resource-type"></a>accessReviewError 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

表示在访问评审实例生命周期中发生的错误。 此资源是只读的。

继承自 [genericError](../resources/genericerror.md)。

## <a name="properties"></a>属性
| 属性                     | 类型     | 说明                          |
| :--------------------------- | :------  | :----------                          |
| code  |String  | 表示错误类型。 继承自 genericError。 只读。 |
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
