---
author: daspek
ms.author: dspektor
title: moveAction 资源类型
description: MoveAction 对象提供有关移动项的活动的信息。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: ec1ac8ccaae502f66e205571e17eb5ad3eced8e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48020529"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="5f295-103">moveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f295-103">moveAction resource type</span></span>

<span data-ttu-id="5f295-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f295-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5f295-105">[**ItemActivity**][activity]上的**moveAction**资源是否存在指示活动已移动项目。</span><span class="sxs-lookup"><span data-stu-id="5f295-105">The presence of the **moveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

><span data-ttu-id="5f295-106">**注意：** 项目活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="5f295-106">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="5f295-107">属性</span><span class="sxs-lookup"><span data-stu-id="5f295-107">Properties</span></span>

| <span data-ttu-id="5f295-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="5f295-108">Property name</span></span> | <span data-ttu-id="5f295-109">类型</span><span class="sxs-lookup"><span data-stu-id="5f295-109">Type</span></span>   | <span data-ttu-id="5f295-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f295-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="5f295-111">from</span><span class="sxs-lookup"><span data-stu-id="5f295-111">from</span></span>          | <span data-ttu-id="5f295-112">string</span><span class="sxs-lookup"><span data-stu-id="5f295-112">string</span></span> | <span data-ttu-id="5f295-113">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="5f295-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="5f295-114">to</span><span class="sxs-lookup"><span data-stu-id="5f295-114">to</span></span>            | <span data-ttu-id="5f295-115">string</span><span class="sxs-lookup"><span data-stu-id="5f295-115">string</span></span> | <span data-ttu-id="5f295-116">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="5f295-116">The name of the location the item was moved to.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f295-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f295-117">JSON representation</span></span>

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

