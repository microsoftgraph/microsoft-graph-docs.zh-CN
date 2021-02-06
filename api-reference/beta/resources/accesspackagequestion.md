---
title: accessPackageQuestion 资源类型
description: 在访问包分配策略上配置的问题的复杂类型。
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 04849b79cfa6c58132360f8ec20c363ea21453ec
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132376"
---
# <a name="accesspackagequestion-resource-type"></a>accessPackageQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 `accessPackageQuestion` 访问包分配 [策略的属性](accesspackageassignmentpolicy.md)。 

子类型包括 [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) 和 [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|字符串| 问题的 ID。|
|isRequired|Boolean| 请求者是否需要提供答案。|
|Sequence|Int32| 向请求者显示问题列表时此问题的相对位置。|
|text|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|要向请求者显示的问题的文本。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer"
}
```

