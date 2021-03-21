---
title: removeProtectionAction 资源类型
description: 表示从文件或信息中删除保护的操作。
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2b315c9d2641524d8a134f0e0b9704c51419ada4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962033"
---
# <a name="removeprotectionaction-resource-type"></a>removeProtectionAction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示从文件或信息中删除保护的操作。 如果由于更新或删除标签而要删除保护，则 evaluateApplication、evaluateClassificationResults 或 [evaluateRemoval](../api/informationprotectionlabel-evaluateremoval.md) API 可能会返回 **removeProtectionAction。** [](../api/informationprotectionlabel-evaluateapplication.md) [](../api/informationprotectionlabel-evaluateclassificationresults.md) 此操作指示使用应用程序删除包含以前适用的内容标头的特定 UI 元素。 只有在调用用户具有删除保护的足够权限时，才应删除通过客户端库（如 Microsoft 信息保护 SDK）的保护。

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

