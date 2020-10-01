---
title: accessReviewRecurrenceSettings 资源类型
description: 指定以固定间隔重复进行访问评审。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ca66a818059efac84903f763e6be3c8a3b5c05a
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330165"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>accessReviewRecurrenceSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AccessReviewRecurrenceSettings**资源类型在[accessReviewSettings](accessreviewsettings.md)资源中使用，并指定以固定间隔重复进行访问评审。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| recurrenceType | 字符串 | 定期间隔。 可能的 vaules： `onetime` 、 `weekly` 、、 `monthly` `quarterly` `halfyearly` 或 `annual` 。                                                                   |
| recurrenceEndType | 字符串 | 重复周期的结束方式。 可能的值： `never` 、、 `endBy` `occurrences` 或 `recurrenceCount` 。 如果是，则不 `never` 会出现定期系列的显式结束。 如果是 `endBy` ，则重复周期将在特定日期结束。 如果是 `occurrences` ，则在审阅的实例完成后，该系列将结束 `recurrenceCount` 。 |
| durationInDays | Int32 | 定期的持续时间（以天为单位）。 |
| recurrenceCount | Int32 | 如果 **recurrenceEndType** 的值为，则为定期计数 `occurrences` ，否则为0。 |

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