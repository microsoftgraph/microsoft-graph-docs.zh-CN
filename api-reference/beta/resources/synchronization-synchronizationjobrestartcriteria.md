---
title: synchronizationJobRestartCriteria 资源类型
description: 定义的范围的[synchronizationJob： 重新启动](../api/synchronization_synchronizationjob_restart.md)操作。
localization_priority: Normal
ms.openlocfilehash: e26bae2e418da22a2b56e3acb973e4111066df23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27867877"
---
# <a name="synchronizationjobrestartcriteria-resource-type"></a>synchronizationJobRestartCriteria 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

定义的范围的[synchronizationJob： 重新启动](../api/synchronization_synchronizationjob_restart.md)操作。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|resetScope|字符串| 以逗号分隔的下列值的组合： `Full`， `QuarantineState`， `Watermark`， `Escrows`， `ConnectorDataStore`。 使用`Full`如果希望所有选项。|

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationJobRestartCriteria resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
