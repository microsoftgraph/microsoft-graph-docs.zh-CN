---
title: plannerTaskDetails 资源类型
description: '**PlannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 6eaeaf65271309270d7ecfd042ed75e5c32451a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965850"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="54918-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="54918-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="54918-105">**PlannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="54918-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="54918-106">每个[任务](plannertask.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="54918-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="54918-107">方法</span><span class="sxs-lookup"><span data-stu-id="54918-107">Methods</span></span>

| <span data-ttu-id="54918-108">方法</span><span class="sxs-lookup"><span data-stu-id="54918-108">Method</span></span>           | <span data-ttu-id="54918-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="54918-109">Return Type</span></span>    |<span data-ttu-id="54918-110">说明</span><span class="sxs-lookup"><span data-stu-id="54918-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="54918-111">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="54918-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="54918-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="54918-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="54918-113">读取**plannerTaskDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="54918-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="54918-114">更新</span><span class="sxs-lookup"><span data-stu-id="54918-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="54918-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="54918-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="54918-116">更新**plannerTaskDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="54918-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="54918-117">属性</span><span class="sxs-lookup"><span data-stu-id="54918-117">Properties</span></span>
| <span data-ttu-id="54918-118">属性</span><span class="sxs-lookup"><span data-stu-id="54918-118">Property</span></span>     | <span data-ttu-id="54918-119">类型</span><span class="sxs-lookup"><span data-stu-id="54918-119">Type</span></span>   |<span data-ttu-id="54918-120">说明</span><span class="sxs-lookup"><span data-stu-id="54918-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54918-121">checklist</span><span class="sxs-lookup"><span data-stu-id="54918-121">checklist</span></span>|[<span data-ttu-id="54918-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="54918-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="54918-123">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="54918-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="54918-124">说明</span><span class="sxs-lookup"><span data-stu-id="54918-124">description</span></span>|<span data-ttu-id="54918-125">String</span><span class="sxs-lookup"><span data-stu-id="54918-125">String</span></span>|<span data-ttu-id="54918-126">任务描述</span><span class="sxs-lookup"><span data-stu-id="54918-126">Description of the task</span></span>|
|<span data-ttu-id="54918-127">id</span><span class="sxs-lookup"><span data-stu-id="54918-127">id</span></span>|<span data-ttu-id="54918-128">String</span><span class="sxs-lookup"><span data-stu-id="54918-128">String</span></span>| <span data-ttu-id="54918-129">只读。</span><span class="sxs-lookup"><span data-stu-id="54918-129">Read-only.</span></span> <span data-ttu-id="54918-130">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="54918-130">ID of the task details.</span></span> <span data-ttu-id="54918-131">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="54918-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="54918-132">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="54918-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="54918-133">previewType</span><span class="sxs-lookup"><span data-stu-id="54918-133">previewType</span></span>|<span data-ttu-id="54918-134">string</span><span class="sxs-lookup"><span data-stu-id="54918-134">string</span></span>|<span data-ttu-id="54918-p104">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="54918-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="54918-138">references</span><span class="sxs-lookup"><span data-stu-id="54918-138">references</span></span>|[<span data-ttu-id="54918-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="54918-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="54918-140">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="54918-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54918-141">关系</span><span class="sxs-lookup"><span data-stu-id="54918-141">Relationships</span></span>
<span data-ttu-id="54918-142">无</span><span class="sxs-lookup"><span data-stu-id="54918-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="54918-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54918-143">JSON representation</span></span>
<span data-ttu-id="54918-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54918-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerTaskDetails"
}-->

```json
{
  "checklist": {"@odata.type": "microsoft.graph.plannerChecklistItems"},
  "description": "String",
  "id": "String (identifier)",
  "previewType": "string",
  "references": {"@odata.type": "microsoft.graph.plannerExternalReferences"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
