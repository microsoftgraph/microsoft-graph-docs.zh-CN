---
title: 'accessReviewRecurrenceSettings 资源类型 (已弃用) '
description: 指定访问评审定期重复进行。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9fa6fb47c541094c85778621289d1abb6d71f727
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821209"
---
# <a name="accessreviewrecurrencesettings-resource-type-deprecated"></a>accessReviewRecurrenceSettings 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

**accessReviewRecurrenceSettings** 资源类型在 [accessReviewSettings](accessreviewsettings.md) 资源中使用，并指定访问评审定期重复。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| recurrenceType | String | 重复间隔。 可能的变体：`onetime`、`weekly`、`monthly`或 `quarterly``halfyearly` `annual`。                                                                   |
| recurrenceEndType | String | 重复性如何结束。 可能的值：`never`、`endBy`或 `occurrences``recurrenceCount`。 如果是 `never`，则重复序列没有显式结束。 如果是 `endBy`，则重复周期在特定日期结束。 如果是 `occurrences`，则序列在审阅实例完成后 `recurrenceCount` 结束。 |
| durationInDays | Int32 | 重复周期的持续时间（以天为单位）。 |
| recurrenceCount | Int32 | 如果 **recurrenceEndType** 的值为 `occurrences`或 `0` 以其他方式表示，则为重复周期计数。 |

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
