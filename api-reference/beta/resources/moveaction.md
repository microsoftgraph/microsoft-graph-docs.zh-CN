---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MoveAction
localization_priority: Normal
ms.openlocfilehash: aa20816165ed4f41e8b89af106e3f781b1be8dd7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29530081"
---
# <a name="moveaction-resource-type"></a><span data-ttu-id="81460-102">MoveAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="81460-102">MoveAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81460-103">[**itemActivity**][activity] 上存在 **MoveAction** 资源指示活动移动了一个项。</span><span class="sxs-lookup"><span data-stu-id="81460-103">The presence of the **MoveAction** resource on an [**itemActivity**][activity] indicates that the activity moved an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="81460-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81460-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="81460-105">属性</span><span class="sxs-lookup"><span data-stu-id="81460-105">Properties</span></span>

| <span data-ttu-id="81460-106">属性名称</span><span class="sxs-lookup"><span data-stu-id="81460-106">Property name</span></span> | <span data-ttu-id="81460-107">类型</span><span class="sxs-lookup"><span data-stu-id="81460-107">Type</span></span>   | <span data-ttu-id="81460-108">说明</span><span class="sxs-lookup"><span data-stu-id="81460-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="81460-109">from</span><span class="sxs-lookup"><span data-stu-id="81460-109">from</span></span>          | <span data-ttu-id="81460-110">string</span><span class="sxs-lookup"><span data-stu-id="81460-110">string</span></span> | <span data-ttu-id="81460-111">被移动项原来位置的名称。</span><span class="sxs-lookup"><span data-stu-id="81460-111">The name of the location the item was moved from.</span></span>
| <span data-ttu-id="81460-112">to</span><span class="sxs-lookup"><span data-stu-id="81460-112">to</span></span>            | <span data-ttu-id="81460-113">string</span><span class="sxs-lookup"><span data-stu-id="81460-113">string</span></span> | <span data-ttu-id="81460-114">将项移动到的位置的名称。</span><span class="sxs-lookup"><span data-stu-id="81460-114">The name of the location the item was moved to.</span></span>

## <a name="remarks"></a><span data-ttu-id="81460-115">注解</span><span class="sxs-lookup"><span data-stu-id="81460-115">Remarks</span></span>

<span data-ttu-id="81460-116">项活动记录当前仅在 SharePoint 和 OneDrive for Business 上可用。</span><span class="sxs-lookup"><span data-stu-id="81460-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The MoveAction object provides information about an activity that moved an item.",
  "keywords": "activities,activity,action,move,moved",
  "section": "documentation",
  "tocPath": "Resources/MoveAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/moveaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
