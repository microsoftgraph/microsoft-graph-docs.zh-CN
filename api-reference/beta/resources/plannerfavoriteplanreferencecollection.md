---
title: plannerFavoritePlanReferenceCollection 资源类型
description: " 值是 plannerFavoritePlanReference 对象。"
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: c473d4101a1247420e641b532ea04dfbc1a26d2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572624"
---
# <a name="plannerfavoriteplanreferencecollection-resource-type"></a>plannerFavoritePlanReferenceCollection 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**plannerFavoritePlanReferenceCollection**资源表示对计划的引用的集合, 这些计划被用户标记为收藏。 此资源是打开的类型, 并且是[plannerUser](planneruser.md)对象的一部分。 属性值对中的属性名称是对应计划的 ID;值是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。


## <a name="properties"></a>属性
您可以定义此开放类型的属性。 属性名称是`id` [plannerPlan](plannerplan.md)资源的值, 它们的值必须是[plannerFavoritePlanReference](plannerfavoriteplanreference.md)对象。 若要删除收藏夹列表中的项, 请将该属性的值设置`null`为。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
}-->

```json
{
  "jd8S5gOaFk2S8aWCIAJz42QAAxtD": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586866870001551087",
    "planTitle": "Customer reviews"
  },
  "uZWtCtli30CGoWLIWSat1mQAC0ai": {
    "@odata.type": "microsoft.graph.plannerFavoritePlanReference",
    "orderHint": "8586848705198093378",
    "planTitle": "Order Management (December 2017)"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerFavoritePlanReferenceCollection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerfavoriteplanreferencecollection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
