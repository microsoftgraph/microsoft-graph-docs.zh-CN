---
title: synchronizationJobRestartCriteria 资源类型
description: '定义[synchronizationJob: restart](../api/synchronization_synchronizationjob_restart.md)操作的范围。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fda28a84f568b9d535a06226397375f3fa8e444a
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620722"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>synchronizationJobRestartCriteria 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

定义[synchronizationJob: restart](../api/synchronization-synchronizationjob-restart.md)操作的范围。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|resetScope|String| 以下`Full`值的逗号分隔组合:、 `QuarantineState` `Watermark` `Escrows`、、。 `ConnectorDataStore` 如果`Full`您想要所有选项, 请使用。|

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
