---
title: 'autoReviewSettings 资源类型 (已弃用) '
description: 指定访问评审完成时的行为。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 593c07266432a389b0f63891675fa9f4823db784
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820257"
---
# <a name="autoreviewsettings-resource-type-deprecated"></a>autoReviewSettings 资源类型 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

**autoReviewSettings** 资源类型在 [accessReviewSettings](accessreviewsettings.md) 资源中使用，并指定访问评审完成时的行为。    

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| notReviewedResult | String | 可能的值：`Approve`或 `Deny``Recommendation`.  如果，则 `Recommendation`**accessReviewSettings** 资源中的 **accessRecommendationsEnabled** 也应设置为 `true`。 如果希望系统提供决策，即使审阅者未做出选择，请将 **accessReviewSettings** 资源中的 **autoReviewEnabled** 属性设置为`true`包含 **notReviewedResult** 属性的 **autoReviewSettings** 对象。 然后，当审阅完成时，根据 **notReviewedResult** 属性，该决定将记录为任 `Approve` 一或 `Deny`。|

## <a name="json-representation"></a>JSON 表示形式

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.autoReviewSettings"
}-->
```json
{
  "notReviewedResult": "string"
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "autoReviewSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
