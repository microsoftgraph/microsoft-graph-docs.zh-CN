---
author: daspek
description: <decription>
ms.date: 09/14/2017
title: RestoreAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: ec2456105c7ae1844f97e80601fe2df3bf38d028
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521087"
---
# <a name="restoreaction-resource-type"></a><span data-ttu-id="e991b-102">RestoreAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="e991b-102">RestoreAction resource type</span></span>

<span data-ttu-id="e991b-103">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e991b-103">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e991b-104">[**itemActivity**][activity] 上存在 **RestoreAction** 资源指示活动还原了一个项。</span><span class="sxs-lookup"><span data-stu-id="e991b-104">The presence of the **RestoreAction** resource on an [**itemActivity**][activity] indicates that the activity restored an item.</span></span>

<span data-ttu-id="e991b-105">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="e991b-105">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e991b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e991b-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.restoreAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="e991b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e991b-107">Properties</span></span>

<span data-ttu-id="e991b-108">无。</span><span class="sxs-lookup"><span data-stu-id="e991b-108">None.</span></span> <span data-ttu-id="e991b-109">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="e991b-109">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="e991b-110">注解</span><span class="sxs-lookup"><span data-stu-id="e991b-110">Remarks</span></span>

<span data-ttu-id="e991b-111">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="e991b-111">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
