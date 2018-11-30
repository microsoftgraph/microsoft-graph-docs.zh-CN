---
title: plannerTaskDetails 资源类型
description: '**plannerTaskDetails** 资源表示任务的其他相关信息。每个任务对象均有一个详细信息对象。'
ms.openlocfilehash: 74ba1c5b7c607f30253463e6cfc256fd3119bf45
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011430"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="0516a-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="0516a-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="0516a-p102">**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="0516a-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="0516a-107">方法</span><span class="sxs-lookup"><span data-stu-id="0516a-107">Methods</span></span>

| <span data-ttu-id="0516a-108">方法</span><span class="sxs-lookup"><span data-stu-id="0516a-108">Method</span></span>           | <span data-ttu-id="0516a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="0516a-109">Return Type</span></span>    |<span data-ttu-id="0516a-110">说明</span><span class="sxs-lookup"><span data-stu-id="0516a-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0516a-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0516a-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="0516a-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0516a-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="0516a-113">读取 **plannerTaskDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0516a-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="0516a-114">Update</span><span class="sxs-lookup"><span data-stu-id="0516a-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="0516a-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="0516a-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="0516a-116">更新 **plannerTaskDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="0516a-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="0516a-117">属性</span><span class="sxs-lookup"><span data-stu-id="0516a-117">Properties</span></span>
| <span data-ttu-id="0516a-118">属性</span><span class="sxs-lookup"><span data-stu-id="0516a-118">Property</span></span>     | <span data-ttu-id="0516a-119">类型</span><span class="sxs-lookup"><span data-stu-id="0516a-119">Type</span></span>   |<span data-ttu-id="0516a-120">说明</span><span class="sxs-lookup"><span data-stu-id="0516a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0516a-121">checklist</span><span class="sxs-lookup"><span data-stu-id="0516a-121">checklist</span></span>|[<span data-ttu-id="0516a-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="0516a-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="0516a-123">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="0516a-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="0516a-124">说明</span><span class="sxs-lookup"><span data-stu-id="0516a-124">description</span></span>|<span data-ttu-id="0516a-125">String</span><span class="sxs-lookup"><span data-stu-id="0516a-125">String</span></span>|<span data-ttu-id="0516a-126">任务描述</span><span class="sxs-lookup"><span data-stu-id="0516a-126">Description of the task</span></span>|
|<span data-ttu-id="0516a-127">id</span><span class="sxs-lookup"><span data-stu-id="0516a-127">id</span></span>|<span data-ttu-id="0516a-128">String</span><span class="sxs-lookup"><span data-stu-id="0516a-128">String</span></span>| <span data-ttu-id="0516a-129">只读。</span><span class="sxs-lookup"><span data-stu-id="0516a-129">Read-only.</span></span> <span data-ttu-id="0516a-130">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="0516a-130">ID of the task details.</span></span> <span data-ttu-id="0516a-131">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="0516a-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="0516a-132">服务上执行[格式验证](planner-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="0516a-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="0516a-133">previewType</span><span class="sxs-lookup"><span data-stu-id="0516a-133">previewType</span></span>|<span data-ttu-id="0516a-134">string</span><span class="sxs-lookup"><span data-stu-id="0516a-134">string</span></span>|<span data-ttu-id="0516a-135">这将设置显示任务的预览的类型。</span><span class="sxs-lookup"><span data-stu-id="0516a-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="0516a-136">可能的值为： `automatic`， `noPreview`， `checklist`， `description`， `reference`。</span><span class="sxs-lookup"><span data-stu-id="0516a-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="0516a-137">当设置为`automatic`显示的预览选择应用程序查看任务。</span><span class="sxs-lookup"><span data-stu-id="0516a-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="0516a-138">references</span><span class="sxs-lookup"><span data-stu-id="0516a-138">references</span></span>|[<span data-ttu-id="0516a-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="0516a-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="0516a-140">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="0516a-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0516a-141">关系</span><span class="sxs-lookup"><span data-stu-id="0516a-141">Relationships</span></span>
<span data-ttu-id="0516a-142">无</span><span class="sxs-lookup"><span data-stu-id="0516a-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0516a-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0516a-143">JSON representation</span></span>
<span data-ttu-id="0516a-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0516a-144">Here is a JSON representation of the resource.</span></span>

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
