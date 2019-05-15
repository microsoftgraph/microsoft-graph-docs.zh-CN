---
author: daspek
ms.author: dspektor
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 525558d040109e637e2f3532d16c308a197e45fb
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970657"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="d46bc-103">moveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="d46bc-103">moveAction resource type</span></span>

<span data-ttu-id="d46bc-104">[activity] [**ItemActivity**]上的**moveAction**资源是否存在指示活动已移动项目。</span><span class="sxs-lookup"><span data-stu-id="d46bc-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="d46bc-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="d46bc-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="d46bc-106">属性</span><span class="sxs-lookup"><span data-stu-id="d46bc-106">Properties</span></span>

| <span data-ttu-id="d46bc-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="d46bc-107">Property name</span></span> | <span data-ttu-id="d46bc-108">类型</span><span class="sxs-lookup"><span data-stu-id="d46bc-108">Type</span></span>   | <span data-ttu-id="d46bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="d46bc-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="d46bc-110">from</span><span class="sxs-lookup"><span data-stu-id="d46bc-110">from</span></span>          | <span data-ttu-id="d46bc-111">string</span><span class="sxs-lookup"><span data-stu-id="d46bc-111">string</span></span> | <span data-ttu-id="d46bc-112">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="d46bc-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="d46bc-113">to</span><span class="sxs-lookup"><span data-stu-id="d46bc-113">to</span></span>            | <span data-ttu-id="d46bc-114">string</span><span class="sxs-lookup"><span data-stu-id="d46bc-114">string</span></span> | <span data-ttu-id="d46bc-115">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="d46bc-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d46bc-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d46bc-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.moveAction"
}-->

```json
{
  "from": "string",
  "to": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": []
}
-->
