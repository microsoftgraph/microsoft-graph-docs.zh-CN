---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**PlannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息（按 task 对象的 "百分比" 字段进行组织的视图，包含未启动的列和 "正在进行中" 和 "完成"）。 每个任务都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 7be6483f127910224b05e05fdf885780d8767176
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521669"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="8418f-104">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="8418f-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

<span data-ttu-id="8418f-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="8418f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8418f-106">**PlannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息（按 task 对象的 "百分比" 字段进行组织的视图，包含未启动的列和 "正在进行中" 和 "完成"）。</span><span class="sxs-lookup"><span data-stu-id="8418f-106">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="8418f-107">每个[任务](plannertask.md)都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="8418f-107">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="8418f-108">方法</span><span class="sxs-lookup"><span data-stu-id="8418f-108">Methods</span></span>

| <span data-ttu-id="8418f-109">方法</span><span class="sxs-lookup"><span data-stu-id="8418f-109">Method</span></span>           | <span data-ttu-id="8418f-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8418f-110">Return Type</span></span>    |<span data-ttu-id="8418f-111">说明</span><span class="sxs-lookup"><span data-stu-id="8418f-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8418f-112">获取 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8418f-112">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="8418f-113">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8418f-113">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="8418f-114">读取**plannerProgressTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8418f-114">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="8418f-115">更新</span><span class="sxs-lookup"><span data-stu-id="8418f-115">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="8418f-116">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="8418f-116">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="8418f-117">更新**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="8418f-117">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8418f-118">属性</span><span class="sxs-lookup"><span data-stu-id="8418f-118">Properties</span></span>
| <span data-ttu-id="8418f-119">属性</span><span class="sxs-lookup"><span data-stu-id="8418f-119">Property</span></span>     | <span data-ttu-id="8418f-120">类型</span><span class="sxs-lookup"><span data-stu-id="8418f-120">Type</span></span>   |<span data-ttu-id="8418f-121">说明</span><span class="sxs-lookup"><span data-stu-id="8418f-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8418f-122">id</span><span class="sxs-lookup"><span data-stu-id="8418f-122">id</span></span>|<span data-ttu-id="8418f-123">字符串</span><span class="sxs-lookup"><span data-stu-id="8418f-123">String</span></span>| <span data-ttu-id="8418f-124">只读。</span><span class="sxs-lookup"><span data-stu-id="8418f-124">Read-only.</span></span> <span data-ttu-id="8418f-125">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="8418f-125">ID of the resource.</span></span> <span data-ttu-id="8418f-126">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="8418f-126">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="8418f-127">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="8418f-127">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="8418f-128">orderHint</span><span class="sxs-lookup"><span data-stu-id="8418f-128">orderHint</span></span>|<span data-ttu-id="8418f-129">String</span><span class="sxs-lookup"><span data-stu-id="8418f-129">String</span></span>|<span data-ttu-id="8418f-p104">用于为任务板“进度”视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="8418f-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="8418f-132">关系</span><span class="sxs-lookup"><span data-stu-id="8418f-132">Relationships</span></span>
<span data-ttu-id="8418f-133">无</span><span class="sxs-lookup"><span data-stu-id="8418f-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8418f-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8418f-134">JSON representation</span></span>
<span data-ttu-id="8418f-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8418f-135">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
