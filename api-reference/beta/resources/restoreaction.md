---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
ms.openlocfilehash: fa92c4667d3421420b203cfc158c94d1b4cf78dd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343582"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="b8470-102">RestoreAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8470-102">RestoreAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8470-103">[**itemActivity**][activity] 上存在 **RestoreAction** 资源指示活动还原了一个项。</span><span class="sxs-lookup"><span data-stu-id="b8470-103">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="b8470-104">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="b8470-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b8470-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8470-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="b8470-106">属性</span><span class="sxs-lookup"><span data-stu-id="b8470-106">Properties</span></span>

<span data-ttu-id="b8470-107">无。</span><span class="sxs-lookup"><span data-stu-id="b8470-107">None.</span></span> <span data-ttu-id="b8470-108">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="b8470-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="b8470-109">注解</span><span class="sxs-lookup"><span data-stu-id="b8470-109">Remarks</span></span>

<span data-ttu-id="b8470-110">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b8470-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The RestoreAction object provides information about an activity that restored an item.",
  "keywords": "activities,activity,action,restore,undelete",
  "section": "documentation",
  "tocPath": "Resources/RestoreAction",
  "suppressions": []
}
-->
