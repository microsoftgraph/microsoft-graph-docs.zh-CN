---
title: accessReviewRecurrenceSettings 资源类型
description: 指定定期重复访问评审。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 208d3e8f8c73c8de98a34aadbd616dc9f268925c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136645"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>accessReviewRecurrenceSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**accessReviewRecurrenceSettings** 资源类型用于 [accessReviewSettings](accessreviewsettings.md)资源，并指定定期重复访问评审。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| recurrenceType | 字符串 | 定期间隔。 可能的 vaules： `onetime` ， ， ， 或 `weekly` `monthly` `quarterly` `halfyearly` `annual` 。                                                                   |
| recurrenceEndType | 字符串 | 重复周期如何结束。 可能的值 `never` `endBy` ：、、 `occurrences` 或 `recurrenceCount` 。 如果是， `never` 则定期系列没有显式结束。 如果是， `endBy` 重复周期将在特定日期结束。 如果是， `occurrences` 则系列在审阅实例完成后 `recurrenceCount` 结束。 |
| durationInDays | Int32 | 定期的持续时间（以天表示）。 |
| recurrenceCount | Int32 | 定期计数（如果 **recurrenceEndType** 的值为 ，否则为 `occurrences` 0）。 |

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
