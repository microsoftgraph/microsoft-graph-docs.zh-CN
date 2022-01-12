---
title: accessPackageQuestion 资源类型
description: 在访问包分配策略上配置的问题的复杂类型。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df4158f7869407772b0c7a8807366d03e2ef7a62
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791943"
---
# <a name="accesspackagequestion-resource-type"></a>accessPackageQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于 `accessPackageQuestion` 访问包分配策略 [的 属性](accesspackageassignmentpolicy.md)。 

子类型包括 [accessPackageTextInputQuestions](accesspackagetextinputquestion.md) 和 [accessPackageMultipleChoiceQuestions](accesspackagemultiplechoicequestion.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String| 问题的 ID。|
|isRequired|Boolean| 请求者是否需要提供答案。|
|Sequence|Int32| 向请求者显示问题列表时此问题的相对位置。|
|text|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|要向请求者显示的问题的文本。|
|isAnswerEditable|Boolean| 指定是否允许请求者编辑问题的答案。|

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