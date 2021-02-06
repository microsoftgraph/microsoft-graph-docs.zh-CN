---
title: accessPackageMultipleChoiceQuestion 资源类型
description: 具有多个选项作为问题答案格式的 accessPackageQuestion 的子类
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 54054edcda2f41ad3f4e1bd29fb807c18709ee1d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137338"
---
# <a name="accesspackagemultiplechoicequestion-resource-type"></a>accessPackageMultipleChoiceQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**accessPackageQuestion 的子项**，它提供请求者必须从中选择答案的多个选项。

继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|allowsMultipleSelection|Boolean|指示请求者是否可以选择多个选项作为其答案。|
|choices|[accessPackageAnswerChoice](../resources/accesspackageanswerchoice.md) 集合|答案选择列表。|
|id|字符串|问题的 ID。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|
|isRequired|Boolean|指示请求者是否需要提供答案。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|
|Sequence|Int32|向请求者显示问题列表时此问题的相对位置。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|
|text|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|要显示请求者的问题的文本。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageMultipleChoiceQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "choices": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerChoice"
    }
  ],
  "allowsMultipleSelection": "Boolean"
}
```
