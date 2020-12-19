---
title: accessPackageTextInputQuestion 资源类型
description: 将文本输入作为问题答案格式的 accessPackageQuestion 的子级。
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8609532e096fb587b4dcf49b8eb624aea314a8c6
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720115"
---
# <a name="accesspackagetextinputquestion-resource-type"></a>accessPackageTextInputQuestion 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将文本输入 **作为答案的 accessPackageQuestion** 的子级。

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

