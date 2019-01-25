---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个**任务**均将有一个与其相关联的 plannerProgressTaskBoardTaskFormat 对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522068"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="447e1-104">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="447e1-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="447e1-p102">**plannerProgressTaskBoardTaskFormat** 资源表示用于在“任务板”的“进度”视图（由任务对象上的 PercentComplete 字段的状态组成的视图，包含“未启动”、“正在进行”和“完成”列）下正确呈现任务的信息。每个[任务](plannertask.md)均将有一个与其相关联的 **plannerProgressTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="447e1-p102">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete). Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="447e1-107">方法</span><span class="sxs-lookup"><span data-stu-id="447e1-107">Methods</span></span>

| <span data-ttu-id="447e1-108">方法</span><span class="sxs-lookup"><span data-stu-id="447e1-108">Method</span></span>           | <span data-ttu-id="447e1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="447e1-109">Return Type</span></span>    |<span data-ttu-id="447e1-110">说明</span><span class="sxs-lookup"><span data-stu-id="447e1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="447e1-111">Get plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="447e1-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="447e1-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="447e1-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="447e1-113">读取 **plannerProgressTaskBoardTaskFormat** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="447e1-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="447e1-114">Update</span><span class="sxs-lookup"><span data-stu-id="447e1-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="447e1-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="447e1-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="447e1-116">更新 **plannerProgressTaskBoardTaskFormat** 对象。</span><span class="sxs-lookup"><span data-stu-id="447e1-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="447e1-117">属性</span><span class="sxs-lookup"><span data-stu-id="447e1-117">Properties</span></span>
| <span data-ttu-id="447e1-118">属性</span><span class="sxs-lookup"><span data-stu-id="447e1-118">Property</span></span>     | <span data-ttu-id="447e1-119">类型</span><span class="sxs-lookup"><span data-stu-id="447e1-119">Type</span></span>   |<span data-ttu-id="447e1-120">说明</span><span class="sxs-lookup"><span data-stu-id="447e1-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="447e1-121">id</span><span class="sxs-lookup"><span data-stu-id="447e1-121">id</span></span>|<span data-ttu-id="447e1-122">String</span><span class="sxs-lookup"><span data-stu-id="447e1-122">String</span></span>| <span data-ttu-id="447e1-123">只读。</span><span class="sxs-lookup"><span data-stu-id="447e1-123">Read-only.</span></span> <span data-ttu-id="447e1-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="447e1-124">ID of the resource.</span></span> <span data-ttu-id="447e1-125">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="447e1-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="447e1-126">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="447e1-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="447e1-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="447e1-127">orderHint</span></span>|<span data-ttu-id="447e1-128">String</span><span class="sxs-lookup"><span data-stu-id="447e1-128">String</span></span>|<span data-ttu-id="447e1-p104">用于对任务板进度视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="447e1-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="447e1-131">关系</span><span class="sxs-lookup"><span data-stu-id="447e1-131">Relationships</span></span>
<span data-ttu-id="447e1-132">无</span><span class="sxs-lookup"><span data-stu-id="447e1-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="447e1-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="447e1-133">JSON representation</span></span>
<span data-ttu-id="447e1-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="447e1-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerProgressTaskBoardTaskFormat"
}-->

```json
{
  "id": "String (identifier)",
  "orderHint": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerprogresstaskboardtaskformat.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
