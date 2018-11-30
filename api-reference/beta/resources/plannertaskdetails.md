---
title: plannerTaskDetails 资源类型
description: '**plannerTaskDetails** 资源表示任务的其他相关信息。每个任务对象均有一个详细信息对象。'
ms.openlocfilehash: 3d5ab0b3a2f0c2e6c1abf284d5a87c2726c7aa15
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049334"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="d7a8a-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7a8a-104">plannerTaskDetails resource type</span></span>

> <span data-ttu-id="d7a8a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d7a8a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d7a8a-p103">**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-p103">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d7a8a-109">方法</span><span class="sxs-lookup"><span data-stu-id="d7a8a-109">Methods</span></span>

| <span data-ttu-id="d7a8a-110">方法</span><span class="sxs-lookup"><span data-stu-id="d7a8a-110">Method</span></span>           | <span data-ttu-id="d7a8a-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="d7a8a-111">Return Type</span></span>    |<span data-ttu-id="d7a8a-112">说明</span><span class="sxs-lookup"><span data-stu-id="d7a8a-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7a8a-113">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d7a8a-113">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="d7a8a-114">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d7a8a-114">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="d7a8a-115">读取 **plannerTaskDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="d7a8a-116">Update</span><span class="sxs-lookup"><span data-stu-id="d7a8a-116">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="d7a8a-117">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d7a8a-117">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="d7a8a-118">更新 **plannerTaskDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-118">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d7a8a-119">属性</span><span class="sxs-lookup"><span data-stu-id="d7a8a-119">Properties</span></span>
| <span data-ttu-id="d7a8a-120">属性</span><span class="sxs-lookup"><span data-stu-id="d7a8a-120">Property</span></span>     | <span data-ttu-id="d7a8a-121">类型</span><span class="sxs-lookup"><span data-stu-id="d7a8a-121">Type</span></span>   |<span data-ttu-id="d7a8a-122">说明</span><span class="sxs-lookup"><span data-stu-id="d7a8a-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7a8a-123">checklist</span><span class="sxs-lookup"><span data-stu-id="d7a8a-123">checklist</span></span>|[<span data-ttu-id="d7a8a-124">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="d7a8a-124">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="d7a8a-125">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-125">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="d7a8a-126">说明</span><span class="sxs-lookup"><span data-stu-id="d7a8a-126">description</span></span>|<span data-ttu-id="d7a8a-127">String</span><span class="sxs-lookup"><span data-stu-id="d7a8a-127">String</span></span>|<span data-ttu-id="d7a8a-128">任务描述</span><span class="sxs-lookup"><span data-stu-id="d7a8a-128">Description of the task</span></span>|
|<span data-ttu-id="d7a8a-129">id</span><span class="sxs-lookup"><span data-stu-id="d7a8a-129">id</span></span>|<span data-ttu-id="d7a8a-130">String</span><span class="sxs-lookup"><span data-stu-id="d7a8a-130">String</span></span>| <span data-ttu-id="d7a8a-131">只读。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-131">Read-only.</span></span> <span data-ttu-id="d7a8a-132">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-132">ID of the task details.</span></span> <span data-ttu-id="d7a8a-133">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-133">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d7a8a-134">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-134">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d7a8a-135">previewType</span><span class="sxs-lookup"><span data-stu-id="d7a8a-135">previewType</span></span>|<span data-ttu-id="d7a8a-136">string</span><span class="sxs-lookup"><span data-stu-id="d7a8a-136">string</span></span>|<span data-ttu-id="d7a8a-p105">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-p105">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="d7a8a-140">references</span><span class="sxs-lookup"><span data-stu-id="d7a8a-140">references</span></span>|[<span data-ttu-id="d7a8a-141">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="d7a8a-141">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="d7a8a-142">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-142">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7a8a-143">关系</span><span class="sxs-lookup"><span data-stu-id="d7a8a-143">Relationships</span></span>
<span data-ttu-id="d7a8a-144">无</span><span class="sxs-lookup"><span data-stu-id="d7a8a-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d7a8a-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7a8a-145">JSON representation</span></span>
<span data-ttu-id="d7a8a-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7a8a-146">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerTaskDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->