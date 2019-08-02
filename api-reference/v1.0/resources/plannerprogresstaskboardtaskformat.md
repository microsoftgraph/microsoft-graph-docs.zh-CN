---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**PlannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息 (按 task 对象的 "百分比" 字段组织的视图, 包含未启动的列)、正在进行和完成)。 每个任务都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6b92cbd231e0cd194b49c11c25d24b93933abbe7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035173"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="86aab-104">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="86aab-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="86aab-105">**PlannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息 (按 task 对象的 "百分比" 字段组织的视图, 包含未启动的列)、正在进行和完成)。</span><span class="sxs-lookup"><span data-stu-id="86aab-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="86aab-106">每个[任务](plannertask.md)都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="86aab-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="86aab-107">方法</span><span class="sxs-lookup"><span data-stu-id="86aab-107">Methods</span></span>

| <span data-ttu-id="86aab-108">方法</span><span class="sxs-lookup"><span data-stu-id="86aab-108">Method</span></span>           | <span data-ttu-id="86aab-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="86aab-109">Return Type</span></span>    |<span data-ttu-id="86aab-110">说明</span><span class="sxs-lookup"><span data-stu-id="86aab-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="86aab-111">获取 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="86aab-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="86aab-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="86aab-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="86aab-113">读取**plannerProgressTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="86aab-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="86aab-114">更新</span><span class="sxs-lookup"><span data-stu-id="86aab-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="86aab-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="86aab-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="86aab-116">更新**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="86aab-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="86aab-117">属性</span><span class="sxs-lookup"><span data-stu-id="86aab-117">Properties</span></span>
| <span data-ttu-id="86aab-118">属性</span><span class="sxs-lookup"><span data-stu-id="86aab-118">Property</span></span>     | <span data-ttu-id="86aab-119">类型</span><span class="sxs-lookup"><span data-stu-id="86aab-119">Type</span></span>   |<span data-ttu-id="86aab-120">说明</span><span class="sxs-lookup"><span data-stu-id="86aab-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86aab-121">id</span><span class="sxs-lookup"><span data-stu-id="86aab-121">id</span></span>|<span data-ttu-id="86aab-122">String</span><span class="sxs-lookup"><span data-stu-id="86aab-122">String</span></span>| <span data-ttu-id="86aab-123">只读。</span><span class="sxs-lookup"><span data-stu-id="86aab-123">Read-only.</span></span> <span data-ttu-id="86aab-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="86aab-124">ID of the resource.</span></span> <span data-ttu-id="86aab-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="86aab-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="86aab-126">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="86aab-126">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="86aab-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="86aab-127">orderHint</span></span>|<span data-ttu-id="86aab-128">String</span><span class="sxs-lookup"><span data-stu-id="86aab-128">String</span></span>|<span data-ttu-id="86aab-p104">用于为任务板“进度”视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="86aab-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="86aab-131">关系</span><span class="sxs-lookup"><span data-stu-id="86aab-131">Relationships</span></span>
<span data-ttu-id="86aab-132">无</span><span class="sxs-lookup"><span data-stu-id="86aab-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="86aab-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86aab-133">JSON representation</span></span>
<span data-ttu-id="86aab-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86aab-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerProgressTaskBoardTaskFormat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
