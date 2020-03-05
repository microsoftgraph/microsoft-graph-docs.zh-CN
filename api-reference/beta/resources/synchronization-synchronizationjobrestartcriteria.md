---
title: synchronizationJobRestartCriteria 资源类型
description: 定义[synchronizationJob： restart](../api/synchronization_synchronizationjob_restart.md)操作的范围。
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c8992104493e7f59b1ddc74c7128dda50b2bfd9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520063"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>synchronizationJobRestartCriteria 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义[synchronizationJob： restart](../api/synchronization-synchronizationjob-restart.md)操作的范围。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|resetScope|String| 以下`Full`值的逗号分隔组合：、 `QuarantineState` `Watermark` `Escrows`、、。 `ConnectorDataStore` 如果`Full`您想要所有选项，请使用。|

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
