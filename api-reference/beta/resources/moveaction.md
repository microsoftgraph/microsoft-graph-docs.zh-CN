---
author: daspek
description: itemActivity 上存在 MoveAction 资源指示活动移动了一个项。
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9fbb19097b6a1401bd3c0b6dba4ce1fd5649e706
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009641"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="7bd50-103">MoveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="7bd50-103">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bd50-104">[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。</span><span class="sxs-lookup"><span data-stu-id="7bd50-104">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7bd50-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7bd50-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7bd50-106">属性</span><span class="sxs-lookup"><span data-stu-id="7bd50-106">Properties</span></span>

| <span data-ttu-id="7bd50-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="7bd50-107">Property name</span></span> | <span data-ttu-id="7bd50-108">类型</span><span class="sxs-lookup"><span data-stu-id="7bd50-108">Type</span></span>   | <span data-ttu-id="7bd50-109">说明</span><span class="sxs-lookup"><span data-stu-id="7bd50-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7bd50-110">from</span><span class="sxs-lookup"><span data-stu-id="7bd50-110">from</span></span>          | <span data-ttu-id="7bd50-111">string</span><span class="sxs-lookup"><span data-stu-id="7bd50-111">string</span></span> | <span data-ttu-id="7bd50-112">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="7bd50-112">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="7bd50-113">to</span><span class="sxs-lookup"><span data-stu-id="7bd50-113">to</span></span>            | <span data-ttu-id="7bd50-114">string</span><span class="sxs-lookup"><span data-stu-id="7bd50-114">string</span></span> | <span data-ttu-id="7bd50-115">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="7bd50-115">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="7bd50-116">注解</span><span class="sxs-lookup"><span data-stu-id="7bd50-116">Remarks</span></span>

<span data-ttu-id="7bd50-117">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="7bd50-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
