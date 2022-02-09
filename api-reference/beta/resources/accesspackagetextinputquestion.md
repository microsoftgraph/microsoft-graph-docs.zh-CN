---
title: accessPackageTextInputQuestion 资源类型
description: 将文本输入作为问题的回答格式的 accessPackageQuestion 的子级。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0dee144139113716257ee1f41b6e585d22dc26b9
ms.sourcegitcommit: 2d61a35735aeb060cc9f7374dd6b50900566293b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2022
ms.locfileid: "62468278"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>accessPackageTextInputQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将文本 **输入作为答案的 accessPackageQuestion** 的子级。  这用于 [accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md) 的 **questions** 属性和访问包资源的 [accessPackageResourceAttribute](accesspackageresourceattribute.md) 中。

继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|问题的 ID。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|
|isRequired|Boolean|指示请求者是否需要提供答案。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|
|isSingleLineQuestion|Boolean|指示答案是单行格式还是多行格式。|
|Sequence|Int32|向请求者显示问题列表时此问题的相对位置。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|
|text|[accessPackageLocalizedContent](../resources/accesspackagelocalizedcontent.md)|要向请求者显示的问题的文本。 继承自 [accessPackageQuestion](../resources/accesspackagequestion.md)。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageTextInputQuestion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageTextInputQuestion",
  "id": "String (identifier)",
  "isRequired": "Boolean",
  "text": {
    "@odata.type": "microsoft.graph.accessPackageLocalizedContent"
  },
  "sequence": "Integer",
  "isSingleLineQuestion": "Boolean"
}
```

