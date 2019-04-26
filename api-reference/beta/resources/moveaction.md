---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 0715f8e9743c4384e8fbd851fe88563e9eaf9666
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342210"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="251a1-102">MoveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="251a1-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="251a1-103">[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。</span><span class="sxs-lookup"><span data-stu-id="251a1-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="251a1-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="251a1-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="251a1-105">属性</span><span class="sxs-lookup"><span data-stu-id="251a1-105">Properties</span></span>

| <span data-ttu-id="251a1-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="251a1-106">Property name</span></span> | <span data-ttu-id="251a1-107">类型</span><span class="sxs-lookup"><span data-stu-id="251a1-107">Type</span></span>   | <span data-ttu-id="251a1-108">说明</span><span class="sxs-lookup"><span data-stu-id="251a1-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="251a1-109">from</span><span class="sxs-lookup"><span data-stu-id="251a1-109">from</span></span>          | <span data-ttu-id="251a1-110">string</span><span class="sxs-lookup"><span data-stu-id="251a1-110">string</span></span> | <span data-ttu-id="251a1-111">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="251a1-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="251a1-112">to</span><span class="sxs-lookup"><span data-stu-id="251a1-112">to</span></span>            | <span data-ttu-id="251a1-113">string</span><span class="sxs-lookup"><span data-stu-id="251a1-113">string</span></span> | <span data-ttu-id="251a1-114">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="251a1-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="251a1-115">注解</span><span class="sxs-lookup"><span data-stu-id="251a1-115">Remarks</span></span>

<span data-ttu-id="251a1-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="251a1-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
