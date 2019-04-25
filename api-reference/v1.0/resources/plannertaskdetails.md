---
title: plannerTaskDetails 资源类型
description: '**plannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 75e17200dc52fff385c7be8fb0269a3da20464b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534323"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="d30a0-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="d30a0-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="d30a0-105">**plannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="d30a0-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="d30a0-106">每个[任务](plannertask.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="d30a0-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="d30a0-107">方法</span><span class="sxs-lookup"><span data-stu-id="d30a0-107">Methods</span></span>

| <span data-ttu-id="d30a0-108">方法</span><span class="sxs-lookup"><span data-stu-id="d30a0-108">Method</span></span>           | <span data-ttu-id="d30a0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d30a0-109">Return Type</span></span>    |<span data-ttu-id="d30a0-110">说明</span><span class="sxs-lookup"><span data-stu-id="d30a0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d30a0-111">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d30a0-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="d30a0-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d30a0-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="d30a0-113">读取**plannerTaskDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d30a0-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="d30a0-114">更新</span><span class="sxs-lookup"><span data-stu-id="d30a0-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="d30a0-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="d30a0-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="d30a0-116">更新**plannerTaskDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="d30a0-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d30a0-117">属性</span><span class="sxs-lookup"><span data-stu-id="d30a0-117">Properties</span></span>
| <span data-ttu-id="d30a0-118">属性</span><span class="sxs-lookup"><span data-stu-id="d30a0-118">Property</span></span>     | <span data-ttu-id="d30a0-119">类型</span><span class="sxs-lookup"><span data-stu-id="d30a0-119">Type</span></span>   |<span data-ttu-id="d30a0-120">说明</span><span class="sxs-lookup"><span data-stu-id="d30a0-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d30a0-121">checklist</span><span class="sxs-lookup"><span data-stu-id="d30a0-121">checklist</span></span>|[<span data-ttu-id="d30a0-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="d30a0-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="d30a0-123">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="d30a0-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="d30a0-124">description</span><span class="sxs-lookup"><span data-stu-id="d30a0-124">description</span></span>|<span data-ttu-id="d30a0-125">String</span><span class="sxs-lookup"><span data-stu-id="d30a0-125">String</span></span>|<span data-ttu-id="d30a0-126">任务描述</span><span class="sxs-lookup"><span data-stu-id="d30a0-126">Description of the task</span></span>|
|<span data-ttu-id="d30a0-127">id</span><span class="sxs-lookup"><span data-stu-id="d30a0-127">id</span></span>|<span data-ttu-id="d30a0-128">String</span><span class="sxs-lookup"><span data-stu-id="d30a0-128">String</span></span>| <span data-ttu-id="d30a0-129">只读。</span><span class="sxs-lookup"><span data-stu-id="d30a0-129">Read-only.</span></span> <span data-ttu-id="d30a0-130">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="d30a0-130">ID of the task details.</span></span> <span data-ttu-id="d30a0-131">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="d30a0-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="d30a0-132">[格式验证](planner-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="d30a0-132">[Format validation](planner-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="d30a0-133">previewType</span><span class="sxs-lookup"><span data-stu-id="d30a0-133">previewType</span></span>|<span data-ttu-id="d30a0-134">string</span><span class="sxs-lookup"><span data-stu-id="d30a0-134">string</span></span>|<span data-ttu-id="d30a0-135">这将设置显示在任务上的预览类型。</span><span class="sxs-lookup"><span data-stu-id="d30a0-135">This sets the type of preview that shows up on the task.</span></span> <span data-ttu-id="d30a0-136">可能的值包括 `automatic`、`noPreview`、`checklist`、`description`、`reference`。</span><span class="sxs-lookup"><span data-stu-id="d30a0-136">The possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.</span></span> <span data-ttu-id="d30a0-137">将设置为`automatic`显示的预览由查看任务的应用程序选择。</span><span class="sxs-lookup"><span data-stu-id="d30a0-137">When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="d30a0-138">references</span><span class="sxs-lookup"><span data-stu-id="d30a0-138">references</span></span>|[<span data-ttu-id="d30a0-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="d30a0-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="d30a0-140">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="d30a0-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d30a0-141">关系</span><span class="sxs-lookup"><span data-stu-id="d30a0-141">Relationships</span></span>
<span data-ttu-id="d30a0-142">无</span><span class="sxs-lookup"><span data-stu-id="d30a0-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d30a0-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d30a0-143">JSON representation</span></span>
<span data-ttu-id="d30a0-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d30a0-144">Here is a JSON representation of the resource.</span></span>

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
