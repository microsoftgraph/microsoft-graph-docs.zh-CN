---
author: daspek
ms.author: dspektor
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 8ef93cd83c8fd020af91a9ea8c9288c1d27d5cf6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036069"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="2cb27-103">moveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="2cb27-103">moveAction resource type</span></span>

<span data-ttu-id="2cb27-104">[**ItemActivity**][activity]上的**moveAction**资源是否存在指示活动已移动项目。</span><span class="sxs-lookup"><span data-stu-id="2cb27-104">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="2cb27-105">**注意:** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="2cb27-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="2cb27-106">属性</span><span class="sxs-lookup"><span data-stu-id="2cb27-106">Properties</span></span>

| <span data-ttu-id="2cb27-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="2cb27-107">Property name</span></span> | <span data-ttu-id="2cb27-108">类型</span><span class="sxs-lookup"><span data-stu-id="2cb27-108">Type</span></span>   | <span data-ttu-id="2cb27-109">说明</span><span class="sxs-lookup"><span data-stu-id="2cb27-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2cb27-110">from</span><span class="sxs-lookup"><span data-stu-id="2cb27-110">from</span></span>          | <span data-ttu-id="2cb27-111">string</span><span class="sxs-lookup"><span data-stu-id="2cb27-111">string</span></span> | <span data-ttu-id="2cb27-112">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="2cb27-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="2cb27-113">to</span><span class="sxs-lookup"><span data-stu-id="2cb27-113">to</span></span>            | <span data-ttu-id="2cb27-114">string</span><span class="sxs-lookup"><span data-stu-id="2cb27-114">string</span></span> | <span data-ttu-id="2cb27-115">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="2cb27-115">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2cb27-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2cb27-116">JSON representation</span></span>

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
