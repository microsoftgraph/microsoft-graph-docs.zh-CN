---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**plannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息 (按 task 对象的 "百分比" 字段组织的视图, 包含未启动的列)、正在进行和完成)。 每个任务都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: ea1382d454a2167df40a37f0da7dbe9b08f867f1
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344364"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="a748c-104">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="a748c-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a748c-105">**plannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息 (按 task 对象的 "百分比" 字段组织的视图, 包含未启动的列)、正在进行和完成)。</span><span class="sxs-lookup"><span data-stu-id="a748c-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="a748c-106">每个[任务](plannertask.md)都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="a748c-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="a748c-107">方法</span><span class="sxs-lookup"><span data-stu-id="a748c-107">Methods</span></span>

| <span data-ttu-id="a748c-108">方法</span><span class="sxs-lookup"><span data-stu-id="a748c-108">Method</span></span>           | <span data-ttu-id="a748c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a748c-109">Return Type</span></span>    |<span data-ttu-id="a748c-110">说明</span><span class="sxs-lookup"><span data-stu-id="a748c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a748c-111">获取 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a748c-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="a748c-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a748c-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="a748c-113">读取**plannerProgressTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a748c-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="a748c-114">更新</span><span class="sxs-lookup"><span data-stu-id="a748c-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="a748c-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="a748c-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="a748c-116">更新**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="a748c-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a748c-117">属性</span><span class="sxs-lookup"><span data-stu-id="a748c-117">Properties</span></span>
| <span data-ttu-id="a748c-118">属性</span><span class="sxs-lookup"><span data-stu-id="a748c-118">Property</span></span>     | <span data-ttu-id="a748c-119">类型</span><span class="sxs-lookup"><span data-stu-id="a748c-119">Type</span></span>   |<span data-ttu-id="a748c-120">说明</span><span class="sxs-lookup"><span data-stu-id="a748c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a748c-121">id</span><span class="sxs-lookup"><span data-stu-id="a748c-121">id</span></span>|<span data-ttu-id="a748c-122">String</span><span class="sxs-lookup"><span data-stu-id="a748c-122">String</span></span>| <span data-ttu-id="a748c-123">只读。</span><span class="sxs-lookup"><span data-stu-id="a748c-123">Read-only.</span></span> <span data-ttu-id="a748c-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="a748c-124">ID of the resource.</span></span> <span data-ttu-id="a748c-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="a748c-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="a748c-126">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="a748c-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="a748c-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="a748c-127">orderHint</span></span>|<span data-ttu-id="a748c-128">String</span><span class="sxs-lookup"><span data-stu-id="a748c-128">String</span></span>|<span data-ttu-id="a748c-p104">用于为任务板“进度”视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="a748c-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a748c-131">关系</span><span class="sxs-lookup"><span data-stu-id="a748c-131">Relationships</span></span>
<span data-ttu-id="a748c-132">无</span><span class="sxs-lookup"><span data-stu-id="a748c-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a748c-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a748c-133">JSON representation</span></span>
<span data-ttu-id="a748c-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a748c-134">Here is a JSON representation of the resource.</span></span>

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
