---
author: daspek
description: itemActivity 上存在 MoveAction 资源指示活动移动了一个项。
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: a42ef869a32cfe01a03344d3f155880bd528c462
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522615"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="8bc9f-103">MoveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bc9f-103">MoveAction resource type</span></span>

<span data-ttu-id="8bc9f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8bc9f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bc9f-105">[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。</span><span class="sxs-lookup"><span data-stu-id="8bc9f-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8bc9f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bc9f-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8bc9f-107">属性</span><span class="sxs-lookup"><span data-stu-id="8bc9f-107">Properties</span></span>

| <span data-ttu-id="8bc9f-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="8bc9f-108">Property name</span></span> | <span data-ttu-id="8bc9f-109">类型</span><span class="sxs-lookup"><span data-stu-id="8bc9f-109">Type</span></span>   | <span data-ttu-id="8bc9f-110">说明</span><span class="sxs-lookup"><span data-stu-id="8bc9f-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8bc9f-111">from</span><span class="sxs-lookup"><span data-stu-id="8bc9f-111">from</span></span>          | <span data-ttu-id="8bc9f-112">string</span><span class="sxs-lookup"><span data-stu-id="8bc9f-112">string</span></span> | <span data-ttu-id="8bc9f-113">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="8bc9f-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="8bc9f-114">to</span><span class="sxs-lookup"><span data-stu-id="8bc9f-114">to</span></span>            | <span data-ttu-id="8bc9f-115">string</span><span class="sxs-lookup"><span data-stu-id="8bc9f-115">string</span></span> | <span data-ttu-id="8bc9f-116">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="8bc9f-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="8bc9f-117">注解</span><span class="sxs-lookup"><span data-stu-id="8bc9f-117">Remarks</span></span>

<span data-ttu-id="8bc9f-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="8bc9f-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
