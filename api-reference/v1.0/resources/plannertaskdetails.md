---
title: plannerTaskDetails 资源类型
description: '**PlannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 32ea3fff1c97920a83f667282e1341926a02b5c1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037373"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="29ac9-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="29ac9-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="29ac9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29ac9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="29ac9-106">**PlannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="29ac9-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="29ac9-107">每个 [任务](plannertask.md) 对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="29ac9-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="29ac9-108">方法</span><span class="sxs-lookup"><span data-stu-id="29ac9-108">Methods</span></span>

| <span data-ttu-id="29ac9-109">方法</span><span class="sxs-lookup"><span data-stu-id="29ac9-109">Method</span></span>           | <span data-ttu-id="29ac9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="29ac9-110">Return Type</span></span>    |<span data-ttu-id="29ac9-111">说明</span><span class="sxs-lookup"><span data-stu-id="29ac9-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="29ac9-112">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="29ac9-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="29ac9-113">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="29ac9-113">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="29ac9-114">读取 **plannerTaskDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29ac9-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="29ac9-115">更新</span><span class="sxs-lookup"><span data-stu-id="29ac9-115">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="29ac9-116">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="29ac9-116">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="29ac9-117">更新 **plannerTaskDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="29ac9-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="29ac9-118">属性</span><span class="sxs-lookup"><span data-stu-id="29ac9-118">Properties</span></span>
| <span data-ttu-id="29ac9-119">属性</span><span class="sxs-lookup"><span data-stu-id="29ac9-119">Property</span></span>     | <span data-ttu-id="29ac9-120">类型</span><span class="sxs-lookup"><span data-stu-id="29ac9-120">Type</span></span>   |<span data-ttu-id="29ac9-121">说明</span><span class="sxs-lookup"><span data-stu-id="29ac9-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="29ac9-122">checklist</span><span class="sxs-lookup"><span data-stu-id="29ac9-122">checklist</span></span>|[<span data-ttu-id="29ac9-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="29ac9-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="29ac9-124">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="29ac9-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="29ac9-125">description</span><span class="sxs-lookup"><span data-stu-id="29ac9-125">description</span></span>|<span data-ttu-id="29ac9-126">String</span><span class="sxs-lookup"><span data-stu-id="29ac9-126">String</span></span>|<span data-ttu-id="29ac9-127">任务描述</span><span class="sxs-lookup"><span data-stu-id="29ac9-127">Description of the task</span></span>|
|<span data-ttu-id="29ac9-128">id</span><span class="sxs-lookup"><span data-stu-id="29ac9-128">id</span></span>|<span data-ttu-id="29ac9-129">String</span><span class="sxs-lookup"><span data-stu-id="29ac9-129">String</span></span>| <span data-ttu-id="29ac9-130">只读。</span><span class="sxs-lookup"><span data-stu-id="29ac9-130">Read-only.</span></span> <span data-ttu-id="29ac9-131">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="29ac9-131">ID of the task details.</span></span> <span data-ttu-id="29ac9-132">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="29ac9-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="29ac9-133">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="29ac9-133">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="29ac9-134">previewType</span><span class="sxs-lookup"><span data-stu-id="29ac9-134">previewType</span></span>|<span data-ttu-id="29ac9-135">string</span><span class="sxs-lookup"><span data-stu-id="29ac9-135">string</span></span>|<span data-ttu-id="29ac9-136">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="29ac9-136">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="29ac9-137">可能的值包括 `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="29ac9-137">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="29ac9-138">将设置为 `automatic` 显示的预览由查看任务的应用程序选择。</span><span class="sxs-lookup"><span data-stu-id="29ac9-138">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="29ac9-139">references</span><span class="sxs-lookup"><span data-stu-id="29ac9-139">references</span></span>|[<span data-ttu-id="29ac9-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="29ac9-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="29ac9-141">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="29ac9-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29ac9-142">关系</span><span class="sxs-lookup"><span data-stu-id="29ac9-142">Relationships</span></span>
<span data-ttu-id="29ac9-143">无</span><span class="sxs-lookup"><span data-stu-id="29ac9-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="29ac9-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="29ac9-144">JSON representation</span></span>
<span data-ttu-id="29ac9-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29ac9-145">Here is a JSON representation of the resource.</span></span>

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

