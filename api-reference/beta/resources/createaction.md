---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
ms.openlocfilehash: 0872e74004fa65f1f1778c6e6123bb3c8af6c823
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509075"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="27d17-102">CreateAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="27d17-102">CreateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27d17-103">[**itemActivity**][activity] 上存在 **CreateAction** 资源指示活动已创建一个项。</span><span class="sxs-lookup"><span data-stu-id="27d17-103">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="27d17-104">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="27d17-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="27d17-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="27d17-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="27d17-106">属性</span><span class="sxs-lookup"><span data-stu-id="27d17-106">Properties</span></span>

<span data-ttu-id="27d17-107">无。</span><span class="sxs-lookup"><span data-stu-id="27d17-107">None.</span></span> <span data-ttu-id="27d17-108">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="27d17-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="27d17-109">注解</span><span class="sxs-lookup"><span data-stu-id="27d17-109">Remarks</span></span>

<span data-ttu-id="27d17-110">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="27d17-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/createaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
