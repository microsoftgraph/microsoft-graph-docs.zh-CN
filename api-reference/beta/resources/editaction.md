---
author: daspek
description: itemActivity 上存在 EditAction 资源指示活动已编辑一个项。
ms.date: 09/14/2017
title: EditAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 374b4f7374ba91360bdaa97e5bc36fb0f5aabbae
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006505"
---
# <a name="editaction-resource-type"></a><span data-ttu-id="21b12-103">EditAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="21b12-103">EditAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21b12-104">[**itemActivity**][activity] 上存在 **EditAction** 资源指示活动已编辑一个项。</span><span class="sxs-lookup"><span data-stu-id="21b12-104">The presence of the **EditAction** resource on an [**itemActivity**][activity] indicates that the activity edited an item.</span></span>

<span data-ttu-id="21b12-105">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="21b12-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="21b12-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21b12-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.editAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="21b12-107">属性</span><span class="sxs-lookup"><span data-stu-id="21b12-107">Properties</span></span>

<span data-ttu-id="21b12-108">无。</span><span class="sxs-lookup"><span data-stu-id="21b12-108">None.</span></span> <span data-ttu-id="21b12-109">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="21b12-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="21b12-110">注解</span><span class="sxs-lookup"><span data-stu-id="21b12-110">Remarks</span></span>

<span data-ttu-id="21b12-111">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="21b12-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The EditAction object provides information about an activity that edited an item.",
  "keywords": "activities,activity,action,edit,modify",
  "section": "documentation",
  "tocPath": "Resources/EditAction",
  "suppressions": []
}
-->
