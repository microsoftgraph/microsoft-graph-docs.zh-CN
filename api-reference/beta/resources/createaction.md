---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CreateAction
localization_priority: Normal
ms.openlocfilehash: 9c704c8416ee37f60afb58205742918ce9e2869f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341006"
---
# <a name="createaction-resource-type"></a><span data-ttu-id="b21fc-102">CreateAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b21fc-102">CreateAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b21fc-103">[**itemActivity**][activity] 上存在 **CreateAction** 资源指示活动已创建一个项。</span><span class="sxs-lookup"><span data-stu-id="b21fc-103">The presence of the **CreateAction** resource on an [**itemActivity**][activity] indicates that the activity created an item.</span></span>

<span data-ttu-id="b21fc-104">**注意**：尽管此资源暂为空，但在今后推出的 API 版本中将在此资源中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="b21fc-104">**Note**: While this resource is empty today, in future API revisions it may be populated with additional properties.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b21fc-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b21fc-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.createAction"
}-->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="b21fc-106">属性</span><span class="sxs-lookup"><span data-stu-id="b21fc-106">Properties</span></span>

<span data-ttu-id="b21fc-107">无。</span><span class="sxs-lookup"><span data-stu-id="b21fc-107">None.</span></span> <span data-ttu-id="b21fc-108">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="b21fc-108">This facet is a null or not-null value and contains no properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="b21fc-109">注解</span><span class="sxs-lookup"><span data-stu-id="b21fc-109">Remarks</span></span>

<span data-ttu-id="b21fc-110">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="b21fc-110">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CreateAction object provides information about the creation of an item.",
  "keywords": "activities,activity,action,create,creation",
  "section": "documentation",
  "tocPath": "Resources/CreateAction",
  "suppressions": []
}
-->
