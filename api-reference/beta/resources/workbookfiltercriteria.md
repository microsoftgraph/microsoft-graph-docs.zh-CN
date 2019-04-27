---
title: workbookFilterCriteria 资源类型
description: 表示应用于列的筛选条件。
localization_priority: Normal
ms.openlocfilehash: 4906a44c88fdd7cb071b4ea994fee609cda1151c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348595"
---
# <a name="workbookfiltercriteria-resource-type"></a>workbookFilterCriteria 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示应用于列的筛选条件。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": {"@odata.type":"microsoft.graph.Json"},
  "icon":{"@odata.type": "microsoft.graph.workbookIcon"},
  "operator":"string"
}
```
