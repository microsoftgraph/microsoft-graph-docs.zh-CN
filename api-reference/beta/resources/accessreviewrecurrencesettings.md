---
title: accessReviewRecurrenceSettings 资源类型
description: 指定定期重复访问评审。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb2a05589bfa92331a213a489bfb2a5129850065
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755656"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>accessReviewRecurrenceSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

**accessReviewRecurrenceSettings** 资源类型在 [accessReviewSettings](accessreviewsettings.md)资源中使用，并指定定期重复访问评审。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| recurrenceType | String | 定期间隔。 可能的模块 `onetime` `weekly` `monthly` ：、、、或 `quarterly` `halfyearly` `annual` 。                                                                   |
| recurrenceEndType | String | 定期的结束时间。 可能的值 `never` `endBy` ：、、 `occurrences` 或 `recurrenceCount` 。 如果是 ， `never` 则定期系列没有显式结束。 如果是 ， `endBy` 则重复周期在特定日期结束。 如果是 ， `occurrences` 则系列将在审阅 `recurrenceCount` 实例完成后结束。 |
| durationInDays | Int32 | 重复周期的持续时间（以天表示）。 |
| recurrenceCount | Int32 | 定期计数（如果 **recurrenceEndType** 的值为 `occurrences` ，否则为 `0` ）。 |

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
```json
{
  "recurrenceType": "string",
  "recurrenceEndType": "string",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewRecurrenceSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
