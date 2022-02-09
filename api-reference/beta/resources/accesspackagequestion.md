---
title: accessPackageQuestion 资源类型
description: 在访问包分配策略上配置的问题的复杂类型。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 22e2cb56461830156d76c10f9e136a62dca4d440
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468305"
---
# <a name="accesspackagequestion-resource-type"></a>accessPackageQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于访问包分配策略的 **accessPackageQuestion** 属性和 **accessPackageResourceAttributeQuestion 中的 accessPackageResourceAttributeQuestion**。[](accesspackageassignmentpolicy.md) [](accesspackageresourceattribute.md)

子类型包括 [accessPackageTextInputQuestion](accesspackagetextinputquestion.md) 和 [accessPackageMultipleChoiceQuestion](accesspackagemultiplechoicequestion.md)。

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