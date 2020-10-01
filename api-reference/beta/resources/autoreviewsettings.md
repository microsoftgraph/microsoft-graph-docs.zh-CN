---
title: autoReviewSettings 资源类型
description: 指定访问评审完成时的行为。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2b9d0a621c4229476e0b3bcdadb869e44422e931
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330318"
---
# <a name="autoreviewsettings-resource-type"></a>autoReviewSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**AutoReviewSettings**资源类型在[accessReviewSettings](accessreviewsettings.md)资源中使用，并指定访问评审完成时的行为。    

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| notReviewedResult | 字符串 | 可能的值： `Approve` 、 `Deny` 或 `Recommendation` 。  如果为 `Recommendation` ，则**accessReviewSettings**资源中的**accessRecommendationsEnabled**也应设置为 `true` 。 如果您希望系统在审阅者不做出选择的情况下也提供决定，请将**accessReviewSettings**资源中的**autoReviewEnabled**属性设置为， `true` 并在**autoReviewSettings**对象中添加**notReviewedResult**属性。 然后，当评审完成时，将根据 **notReviewedResult** 属性，将决策记录为 `Approve` 或 `Deny` 。|

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