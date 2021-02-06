---
title: autoReviewSettings 资源类型
description: 指定访问评审完成时的行为。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f46ef4b57a921cc08fbb8f3768597eef12c1ce4f
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136930"
---
# <a name="autoreviewsettings-resource-type"></a>autoReviewSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**autoReviewSettings** 资源类型在 [accessReviewSettings](accessreviewsettings.md)资源中使用，并指定访问评审完成时的行为。    

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
| :------- | :--- | :---------- |
| notReviewedResult | 字符串 | 可能的值： `Approve` ， `Deny` 或 `Recommendation` 。  If `Recommendation` ， then **accessRecommendationsEnabled** in the **accessReviewSettings** resource should also be set to `true` . 如果希望系统提供决策，即使审阅者未做出选择，将 **accessReviewSettings** 资源中的 **autoReviewEnabled** 属性设置为包含 `true` 具有 **notReviewedResult** 属性的 **autoReviewSettings** 对象。 然后，当审阅完成时，基于 **notReviewedResult** 属性，将决定记录为或 `Approve` `Deny` 。|

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
