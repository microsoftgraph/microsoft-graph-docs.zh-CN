---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
ms.openlocfilehash: e319f6889b520f90d9414c4115060edbe2e2f0cc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543042"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="9d19a-102">EditAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d19a-102">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d19a-103">[**itemActivity**][activity] 上存在 **EditAction** 资源指示活动已编辑一个项。</span><span class="sxs-lookup"><span data-stu-id="9d19a-103">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="9d19a-104">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="9d19a-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="9d19a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d19a-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="9d19a-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d19a-106">Properties</span></span>

<span data-ttu-id="9d19a-107">无。</span><span class="sxs-lookup"><span data-stu-id="9d19a-107">None.</span></span> <span data-ttu-id="9d19a-108">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="9d19a-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="9d19a-109">注解</span><span class="sxs-lookup"><span data-stu-id="9d19a-109">Remarks</span></span>

<span data-ttu-id="9d19a-110">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="9d19a-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/editaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
