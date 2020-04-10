---
title: synchronizationJobRestartCriteria 资源类型
description: 定义 synchronizationJob： restart 操作的范围。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f9e8dba8829e7f5340a3ba43d8d9a31df4f98049
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217519"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>synchronizationJobRestartCriteria 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义[synchronizationJob： restart](../api/synchronization-synchronizationjob-restart.md)操作的范围。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|resetScope|字符串| 以下`Full`值的逗号分隔组合：、 `QuarantineState` `Watermark` `Escrows`、、。 `ConnectorDataStore` 如果`Full`您想要所有选项，请使用。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationJobRestartCriteria"
}-->

```json
{
  "resetScope": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
