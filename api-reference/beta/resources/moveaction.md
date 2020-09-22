---
author: daspek
description: itemActivity 上存在 MoveAction 资源指示活动移动了一个项。
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 547a49e17a74be43500a9cf52aaa3a375272b810
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48021285"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="d1b89-103">MoveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1b89-103">MoveAction resource type</span></span>

<span data-ttu-id="d1b89-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1b89-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d1b89-105">[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。</span><span class="sxs-lookup"><span data-stu-id="d1b89-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="d1b89-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1b89-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d1b89-107">属性</span><span class="sxs-lookup"><span data-stu-id="d1b89-107">Properties</span></span>

| <span data-ttu-id="d1b89-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="d1b89-108">Property name</span></span> | <span data-ttu-id="d1b89-109">类型</span><span class="sxs-lookup"><span data-stu-id="d1b89-109">Type</span></span>   | <span data-ttu-id="d1b89-110">说明</span><span class="sxs-lookup"><span data-stu-id="d1b89-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="d1b89-111">from</span><span class="sxs-lookup"><span data-stu-id="d1b89-111">from</span></span>          | <span data-ttu-id="d1b89-112">string</span><span class="sxs-lookup"><span data-stu-id="d1b89-112">string</span></span> | <span data-ttu-id="d1b89-113">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="d1b89-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="d1b89-114">to</span><span class="sxs-lookup"><span data-stu-id="d1b89-114">to</span></span>            | <span data-ttu-id="d1b89-115">string</span><span class="sxs-lookup"><span data-stu-id="d1b89-115">string</span></span> | <span data-ttu-id="d1b89-116">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="d1b89-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="d1b89-117">注解</span><span class="sxs-lookup"><span data-stu-id="d1b89-117">Remarks</span></span>

<span data-ttu-id="d1b89-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="d1b89-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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


