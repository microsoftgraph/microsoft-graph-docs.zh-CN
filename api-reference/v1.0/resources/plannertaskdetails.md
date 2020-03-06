---
title: plannerTaskDetails 资源类型
description: '**PlannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 4dda174401ebf3435c7a190a3f92167ac6b47c0d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533977"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="6cd62-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="6cd62-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="6cd62-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cd62-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6cd62-106">**PlannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="6cd62-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="6cd62-107">每个[任务](plannertask.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="6cd62-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="6cd62-108">Methods</span><span class="sxs-lookup"><span data-stu-id="6cd62-108">Methods</span></span>

| <span data-ttu-id="6cd62-109">方法</span><span class="sxs-lookup"><span data-stu-id="6cd62-109">Method</span></span>           | <span data-ttu-id="6cd62-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6cd62-110">Return Type</span></span>    |<span data-ttu-id="6cd62-111">说明</span><span class="sxs-lookup"><span data-stu-id="6cd62-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cd62-112">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6cd62-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="6cd62-113">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6cd62-113">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="6cd62-114">读取**plannerTaskDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6cd62-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="6cd62-115">更新</span><span class="sxs-lookup"><span data-stu-id="6cd62-115">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="6cd62-116">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="6cd62-116">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="6cd62-117">更新**plannerTaskDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="6cd62-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="6cd62-118">属性</span><span class="sxs-lookup"><span data-stu-id="6cd62-118">Properties</span></span>
| <span data-ttu-id="6cd62-119">属性</span><span class="sxs-lookup"><span data-stu-id="6cd62-119">Property</span></span>     | <span data-ttu-id="6cd62-120">类型</span><span class="sxs-lookup"><span data-stu-id="6cd62-120">Type</span></span>   |<span data-ttu-id="6cd62-121">说明</span><span class="sxs-lookup"><span data-stu-id="6cd62-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cd62-122">checklist</span><span class="sxs-lookup"><span data-stu-id="6cd62-122">checklist</span></span>|[<span data-ttu-id="6cd62-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="6cd62-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="6cd62-124">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="6cd62-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="6cd62-125">说明</span><span class="sxs-lookup"><span data-stu-id="6cd62-125">description</span></span>|<span data-ttu-id="6cd62-126">字符串</span><span class="sxs-lookup"><span data-stu-id="6cd62-126">String</span></span>|<span data-ttu-id="6cd62-127">任务描述</span><span class="sxs-lookup"><span data-stu-id="6cd62-127">Description of the task</span></span>|
|<span data-ttu-id="6cd62-128">id</span><span class="sxs-lookup"><span data-stu-id="6cd62-128">id</span></span>|<span data-ttu-id="6cd62-129">字符串</span><span class="sxs-lookup"><span data-stu-id="6cd62-129">String</span></span>| <span data-ttu-id="6cd62-130">只读。</span><span class="sxs-lookup"><span data-stu-id="6cd62-130">Read-only.</span></span> <span data-ttu-id="6cd62-131">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="6cd62-131">ID of the task details.</span></span> <span data-ttu-id="6cd62-132">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="6cd62-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="6cd62-133">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="6cd62-133">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="6cd62-134">previewType</span><span class="sxs-lookup"><span data-stu-id="6cd62-134">previewType</span></span>|<span data-ttu-id="6cd62-135">string</span><span class="sxs-lookup"><span data-stu-id="6cd62-135">string</span></span>|<span data-ttu-id="6cd62-136">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="6cd62-136">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="6cd62-137">可能的值包括 `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="6cd62-137">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="6cd62-138">将设置为`automatic`显示的预览由查看任务的应用程序选择。</span><span class="sxs-lookup"><span data-stu-id="6cd62-138">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="6cd62-139">references</span><span class="sxs-lookup"><span data-stu-id="6cd62-139">references</span></span>|[<span data-ttu-id="6cd62-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="6cd62-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="6cd62-141">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="6cd62-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cd62-142">关系</span><span class="sxs-lookup"><span data-stu-id="6cd62-142">Relationships</span></span>
<span data-ttu-id="6cd62-143">无</span><span class="sxs-lookup"><span data-stu-id="6cd62-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6cd62-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cd62-144">JSON representation</span></span>
<span data-ttu-id="6cd62-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cd62-145">Here is a JSON representation of the resource.</span></span>

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
