---
author: daspek
ms.author: dspektor
ms.date: 09/12/2018
title: AccessAction
localization_priority: Normal
ms.openlocfilehash: bef6444fd42080c6f5b7cdabb69dbe9a50bab8d6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511518"
---
# <a name="accessaction-resource-type"></a><span data-ttu-id="20ea0-102">accessAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="20ea0-102">accessAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20ea0-103">上[**itemActivity**] **accessAction**资源的状态[activity]指示活动的正访问项。</span><span class="sxs-lookup"><span data-stu-id="20ea0-103">The presence of the **accessAction** resource on an [**itemActivity**][activity] indicates that the activity accessed an item.</span></span>

><span data-ttu-id="20ea0-104">**注意：** Access 活动记录才当前 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="20ea0-104">**Note:** Access activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="20ea0-105">属性</span><span class="sxs-lookup"><span data-stu-id="20ea0-105">Properties</span></span>

<span data-ttu-id="20ea0-106">此资源类型有任何属性。</span><span class="sxs-lookup"><span data-stu-id="20ea0-106">This resource type has no properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20ea0-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20ea0-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.accessAction"
}-->

```json
{
}
```


<!--
{
  "type": "#page.annotation",
  "description": "The AccessAction object provides information about accesses of an item.",
  "keywords": "activities,activity,action,access",
  "section": "documentation",
  "tocPath": "Resources/AccessAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/accessaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
