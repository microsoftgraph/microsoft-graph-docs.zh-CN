---
title: plannerTaskDetails 资源类型
description: '**PlannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: d22c932989b9c0d21350842babd9b4bbf420124c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035166"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="f1342-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="f1342-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="f1342-105">**PlannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="f1342-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="f1342-106">每个[任务](plannertask.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="f1342-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="f1342-107">方法</span><span class="sxs-lookup"><span data-stu-id="f1342-107">Methods</span></span>

| <span data-ttu-id="f1342-108">方法</span><span class="sxs-lookup"><span data-stu-id="f1342-108">Method</span></span>           | <span data-ttu-id="f1342-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f1342-109">Return Type</span></span>    |<span data-ttu-id="f1342-110">说明</span><span class="sxs-lookup"><span data-stu-id="f1342-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f1342-111">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f1342-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="f1342-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f1342-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="f1342-113">读取**plannerTaskDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f1342-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="f1342-114">更新</span><span class="sxs-lookup"><span data-stu-id="f1342-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="f1342-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f1342-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="f1342-116">更新**plannerTaskDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="f1342-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f1342-117">属性</span><span class="sxs-lookup"><span data-stu-id="f1342-117">Properties</span></span>
| <span data-ttu-id="f1342-118">属性</span><span class="sxs-lookup"><span data-stu-id="f1342-118">Property</span></span>     | <span data-ttu-id="f1342-119">类型</span><span class="sxs-lookup"><span data-stu-id="f1342-119">Type</span></span>   |<span data-ttu-id="f1342-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1342-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1342-121">checklist</span><span class="sxs-lookup"><span data-stu-id="f1342-121">checklist</span></span>|[<span data-ttu-id="f1342-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="f1342-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="f1342-123">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="f1342-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="f1342-124">说明</span><span class="sxs-lookup"><span data-stu-id="f1342-124">description</span></span>|<span data-ttu-id="f1342-125">字符串</span><span class="sxs-lookup"><span data-stu-id="f1342-125">String</span></span>|<span data-ttu-id="f1342-126">任务描述</span><span class="sxs-lookup"><span data-stu-id="f1342-126">Description of the task</span></span>|
|<span data-ttu-id="f1342-127">id</span><span class="sxs-lookup"><span data-stu-id="f1342-127">id</span></span>|<span data-ttu-id="f1342-128">字符串</span><span class="sxs-lookup"><span data-stu-id="f1342-128">String</span></span>| <span data-ttu-id="f1342-129">只读。</span><span class="sxs-lookup"><span data-stu-id="f1342-129">Read-only.</span></span> <span data-ttu-id="f1342-130">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="f1342-130">ID of the task details.</span></span> <span data-ttu-id="f1342-131">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="f1342-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f1342-132">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="f1342-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="f1342-133">previewType</span><span class="sxs-lookup"><span data-stu-id="f1342-133">previewType</span></span>|<span data-ttu-id="f1342-134">string</span><span class="sxs-lookup"><span data-stu-id="f1342-134">string</span></span>|<span data-ttu-id="f1342-135">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="f1342-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="f1342-136">可能的值包括 `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="f1342-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="f1342-137">将设置为`automatic`显示的预览由查看任务的应用程序选择。</span><span class="sxs-lookup"><span data-stu-id="f1342-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="f1342-138">references</span><span class="sxs-lookup"><span data-stu-id="f1342-138">references</span></span>|[<span data-ttu-id="f1342-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="f1342-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="f1342-140">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="f1342-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f1342-141">关系</span><span class="sxs-lookup"><span data-stu-id="f1342-141">Relationships</span></span>
<span data-ttu-id="f1342-142">无</span><span class="sxs-lookup"><span data-stu-id="f1342-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f1342-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f1342-143">JSON representation</span></span>
<span data-ttu-id="f1342-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f1342-144">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
