---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: 40049b506c72af5aacddf461b22e1ddd280d7ad4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852897"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="1def1-102">MoveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="1def1-102">MoveAction resource type</span></span>

> <span data-ttu-id="1def1-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1def1-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1def1-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1def1-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1def1-105">[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。</span><span class="sxs-lookup"><span data-stu-id="1def1-105">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="1def1-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1def1-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1def1-107">属性</span><span class="sxs-lookup"><span data-stu-id="1def1-107">Properties</span></span>

| <span data-ttu-id="1def1-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="1def1-108">Property name</span></span> | <span data-ttu-id="1def1-109">类型</span><span class="sxs-lookup"><span data-stu-id="1def1-109">Type</span></span>   | <span data-ttu-id="1def1-110">说明</span><span class="sxs-lookup"><span data-stu-id="1def1-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1def1-111">from</span><span class="sxs-lookup"><span data-stu-id="1def1-111">from</span></span>          | <span data-ttu-id="1def1-112">string</span><span class="sxs-lookup"><span data-stu-id="1def1-112">string</span></span> | <span data-ttu-id="1def1-113">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="1def1-113">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="1def1-114">to</span><span class="sxs-lookup"><span data-stu-id="1def1-114">to</span></span>            | <span data-ttu-id="1def1-115">string</span><span class="sxs-lookup"><span data-stu-id="1def1-115">string</span></span> | <span data-ttu-id="1def1-116">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="1def1-116">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="1def1-117">注解</span><span class="sxs-lookup"><span data-stu-id="1def1-117">Remarks</span></span>

<span data-ttu-id="1def1-118">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="1def1-118">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction"
} -->
