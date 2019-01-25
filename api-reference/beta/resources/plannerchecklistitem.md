---
title: plannerChecklistItem 资源类型
description: '**plannerChecklistItem** 资源表示任务的检查表中的项目。任务上的检查表由 checklistItems 对象表示。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 87f7349e20245068a0a29a179ddb5505cd3be0ec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522537"
---
# <a name="plannerchecklistitem-resource-type"></a><span data-ttu-id="a9d82-104">plannerChecklistItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="a9d82-104">plannerChecklistItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9d82-p102">**plannerChecklistItem** 资源表示任务的检查表中的项目。任务上的检查表由 [checklistItems 对象](plannerchecklistitems.md)表示。</span><span class="sxs-lookup"><span data-stu-id="a9d82-p102">The **plannerChecklistItem** resource represents an item in the checklist of a task. The checklist on a task is represented by the [checklistItems object](plannerchecklistitems.md).</span></span>


## <a name="properties"></a><span data-ttu-id="a9d82-107">属性</span><span class="sxs-lookup"><span data-stu-id="a9d82-107">Properties</span></span>
| <span data-ttu-id="a9d82-108">属性</span><span class="sxs-lookup"><span data-stu-id="a9d82-108">Property</span></span>     | <span data-ttu-id="a9d82-109">类型</span><span class="sxs-lookup"><span data-stu-id="a9d82-109">Type</span></span>   |<span data-ttu-id="a9d82-110">说明</span><span class="sxs-lookup"><span data-stu-id="a9d82-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a9d82-111">isChecked</span><span class="sxs-lookup"><span data-stu-id="a9d82-111">isChecked</span></span>|<span data-ttu-id="a9d82-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9d82-112">Boolean</span></span>|<span data-ttu-id="a9d82-113">如果已检查此项目，值则为 `true`，否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="a9d82-113">Value is `true` if the item is checked and `false` otherwise.</span></span>|
|<span data-ttu-id="a9d82-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a9d82-114">lastModifiedBy</span></span>|[<span data-ttu-id="a9d82-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="a9d82-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="a9d82-p103">只读。上一次修改它的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="a9d82-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="a9d82-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9d82-118">lastModifiedDateTime</span></span>|<span data-ttu-id="a9d82-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9d82-119">DateTimeOffset</span></span>|<span data-ttu-id="a9d82-p104">只读。上一次修改它的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a9d82-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a9d82-124">orderHint</span><span class="sxs-lookup"><span data-stu-id="a9d82-124">orderHint</span></span>|<span data-ttu-id="a9d82-125">String</span><span class="sxs-lookup"><span data-stu-id="a9d82-125">String</span></span>|<span data-ttu-id="a9d82-p105">用于设置检查表中的项目的相对顺序。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="a9d82-p105">Used to set the relative order of items in the checklist. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|
|<span data-ttu-id="a9d82-128">title</span><span class="sxs-lookup"><span data-stu-id="a9d82-128">title</span></span>|<span data-ttu-id="a9d82-129">String</span><span class="sxs-lookup"><span data-stu-id="a9d82-129">String</span></span>|<span data-ttu-id="a9d82-130">检查表项目的标题</span><span class="sxs-lookup"><span data-stu-id="a9d82-130">Title of the checklist item</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a9d82-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a9d82-131">JSON representation</span></span>
<span data-ttu-id="a9d82-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9d82-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerChecklistItem"
}-->

```json
{
  "isChecked": true,
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "orderHint": "String",
  "title": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerChecklistItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerchecklistitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
