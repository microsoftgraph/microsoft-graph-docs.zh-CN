---
title: removeProtectionAction 资源类型
description: 表示要移除其对文件的保护的操作或信息。
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63a539fe4366703aaeb7e6b16735bb0302951dd7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521143"
---
# <a name="removeprotectionaction-resource-type"></a>removeProtectionAction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示要移除其对文件的保护的操作或信息。 [EvaluateApplication](../api/informationprotectionlabel-evaluateapplication.md)、 [evaluateClassificationResults](../api/informationprotectionlabel-evaluateclassificationresults.md)或[EvaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) api 可能会返回**removeProtectionAction** ，如果由于更新或删除标签而要删除保护。 该操作指示使用应用程序移除包含之前适用的内容头的特定 UI 元素。 仅当呼叫用户具有足够的权限删除保护时，才应通过客户端库（如 Microsoft 信息保护 SDK）删除保护。

## <a name="properties"></a>属性

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.removeProtectionAction",
  "baseType": "microsoft.graph.informationProtectionAction"
}-->

```json
{
  
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "removeProtectionAction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->