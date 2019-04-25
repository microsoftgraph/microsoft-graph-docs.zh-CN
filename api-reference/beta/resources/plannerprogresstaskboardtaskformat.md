---
title: plannerProgressTaskBoardTaskFormat 资源类型
description: '**plannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息 (按 task 对象的 "百分比" 字段组织的视图, 包含未启动的列)、正在进行和完成)。 每个任务都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 20a215b108ca1f1801702a532bda09eac67834c6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522123"
---
# <a name="plannerprogresstaskboardtaskformat-resource-type"></a><span data-ttu-id="c82d5-104">plannerProgressTaskBoardTaskFormat 资源类型</span><span class="sxs-lookup"><span data-stu-id="c82d5-104">plannerProgressTaskBoardTaskFormat resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c82d5-105">**plannerProgressTaskBoardTaskFormat**资源表示用于在任务板的进度视图中正确呈现任务的信息 (按 task 对象的 "百分比" 字段组织的视图, 包含未启动的列)、正在进行和完成)。</span><span class="sxs-lookup"><span data-stu-id="c82d5-105">The **plannerProgressTaskBoardTaskFormat** resource represents the information used to render a task correctly in the Progress view of the Task Board (a view organized by the state of the PercentComplete field on the task object, with columns for Not Started, In Progress and Complete).</span></span> <span data-ttu-id="c82d5-106">每个[任务](plannertask.md)都有一个与之关联的**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="c82d5-106">Each [task](plannertask.md) will have one **plannerProgressTaskBoardTaskFormat** object associated with it.</span></span>


## <a name="methods"></a><span data-ttu-id="c82d5-107">方法</span><span class="sxs-lookup"><span data-stu-id="c82d5-107">Methods</span></span>

| <span data-ttu-id="c82d5-108">方法</span><span class="sxs-lookup"><span data-stu-id="c82d5-108">Method</span></span>           | <span data-ttu-id="c82d5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c82d5-109">Return Type</span></span>    |<span data-ttu-id="c82d5-110">说明</span><span class="sxs-lookup"><span data-stu-id="c82d5-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c82d5-111">获取 plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c82d5-111">Get plannerProgressTaskBoardTaskFormat</span></span>](../api/plannerprogresstaskboardtaskformat-get.md) | [<span data-ttu-id="c82d5-112">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c82d5-112">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md) |<span data-ttu-id="c82d5-113">读取**plannerProgressTaskBoardTaskFormat**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c82d5-113">Read properties and relationships of **plannerProgressTaskBoardTaskFormat** object.</span></span>|
|[<span data-ttu-id="c82d5-114">更新</span><span class="sxs-lookup"><span data-stu-id="c82d5-114">Update</span></span>](../api/plannerprogresstaskboardtaskformat-update.md) | [<span data-ttu-id="c82d5-115">plannerProgressTaskBoardTaskFormat</span><span class="sxs-lookup"><span data-stu-id="c82d5-115">plannerProgressTaskBoardTaskFormat</span></span>](plannerprogresstaskboardtaskformat.md)    |<span data-ttu-id="c82d5-116">更新**plannerProgressTaskBoardTaskFormat**对象。</span><span class="sxs-lookup"><span data-stu-id="c82d5-116">Update **plannerProgressTaskBoardTaskFormat** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c82d5-117">属性</span><span class="sxs-lookup"><span data-stu-id="c82d5-117">Properties</span></span>
| <span data-ttu-id="c82d5-118">属性</span><span class="sxs-lookup"><span data-stu-id="c82d5-118">Property</span></span>     | <span data-ttu-id="c82d5-119">类型</span><span class="sxs-lookup"><span data-stu-id="c82d5-119">Type</span></span>   |<span data-ttu-id="c82d5-120">说明</span><span class="sxs-lookup"><span data-stu-id="c82d5-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c82d5-121">id</span><span class="sxs-lookup"><span data-stu-id="c82d5-121">id</span></span>|<span data-ttu-id="c82d5-122">String</span><span class="sxs-lookup"><span data-stu-id="c82d5-122">String</span></span>| <span data-ttu-id="c82d5-123">只读。</span><span class="sxs-lookup"><span data-stu-id="c82d5-123">Read-only.</span></span> <span data-ttu-id="c82d5-124">资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="c82d5-124">ID of the resource.</span></span> <span data-ttu-id="c82d5-125">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="c82d5-125">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="c82d5-126">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="c82d5-126">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="c82d5-127">orderHint</span><span class="sxs-lookup"><span data-stu-id="c82d5-127">orderHint</span></span>|<span data-ttu-id="c82d5-128">String</span><span class="sxs-lookup"><span data-stu-id="c82d5-128">String</span></span>|<span data-ttu-id="c82d5-p104">用于为任务板“进度”视图上的任务进行排序的提示值。[此处](planner-order-hint-format.md)概述了此格式。</span><span class="sxs-lookup"><span data-stu-id="c82d5-p104">Hint value used to order the task on the Progress view of the Task Board. The format is defined as outlined [here](planner-order-hint-format.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="c82d5-131">关系</span><span class="sxs-lookup"><span data-stu-id="c82d5-131">Relationships</span></span>
<span data-ttu-id="c82d5-132">无</span><span class="sxs-lookup"><span data-stu-id="c82d5-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c82d5-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c82d5-133">JSON representation</span></span>
<span data-ttu-id="c82d5-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c82d5-134">Here is a JSON representation of the resource.</span></span>

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
