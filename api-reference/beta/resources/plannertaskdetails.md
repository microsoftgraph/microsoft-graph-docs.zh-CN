---
title: plannerTaskDetails 资源类型
description: '**PlannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 00d1360435f38cdf22547e5f509b46c931cb50b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521641"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="f368e-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="f368e-104">plannerTaskDetails resource type</span></span>

<span data-ttu-id="f368e-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f368e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f368e-106">**PlannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="f368e-106">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="f368e-107">每个[任务](plannertask.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="f368e-107">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="f368e-108">方法</span><span class="sxs-lookup"><span data-stu-id="f368e-108">Methods</span></span>

| <span data-ttu-id="f368e-109">方法</span><span class="sxs-lookup"><span data-stu-id="f368e-109">Method</span></span>           | <span data-ttu-id="f368e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f368e-110">Return Type</span></span>    |<span data-ttu-id="f368e-111">说明</span><span class="sxs-lookup"><span data-stu-id="f368e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f368e-112">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f368e-112">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="f368e-113">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f368e-113">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="f368e-114">读取**plannerTaskDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f368e-114">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="f368e-115">更新</span><span class="sxs-lookup"><span data-stu-id="f368e-115">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="f368e-116">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="f368e-116">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="f368e-117">更新**plannerTaskDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="f368e-117">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f368e-118">属性</span><span class="sxs-lookup"><span data-stu-id="f368e-118">Properties</span></span>
| <span data-ttu-id="f368e-119">属性</span><span class="sxs-lookup"><span data-stu-id="f368e-119">Property</span></span>     | <span data-ttu-id="f368e-120">类型</span><span class="sxs-lookup"><span data-stu-id="f368e-120">Type</span></span>   |<span data-ttu-id="f368e-121">说明</span><span class="sxs-lookup"><span data-stu-id="f368e-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f368e-122">checklist</span><span class="sxs-lookup"><span data-stu-id="f368e-122">checklist</span></span>|[<span data-ttu-id="f368e-123">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="f368e-123">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="f368e-124">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="f368e-124">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="f368e-125">说明</span><span class="sxs-lookup"><span data-stu-id="f368e-125">description</span></span>|<span data-ttu-id="f368e-126">String</span><span class="sxs-lookup"><span data-stu-id="f368e-126">String</span></span>|<span data-ttu-id="f368e-127">任务描述</span><span class="sxs-lookup"><span data-stu-id="f368e-127">Description of the task</span></span>|
|<span data-ttu-id="f368e-128">id</span><span class="sxs-lookup"><span data-stu-id="f368e-128">id</span></span>|<span data-ttu-id="f368e-129">字符串</span><span class="sxs-lookup"><span data-stu-id="f368e-129">String</span></span>| <span data-ttu-id="f368e-130">只读。</span><span class="sxs-lookup"><span data-stu-id="f368e-130">Read-only.</span></span> <span data-ttu-id="f368e-131">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="f368e-131">ID of the task details.</span></span> <span data-ttu-id="f368e-132">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="f368e-132">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="f368e-133">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="f368e-133">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="f368e-134">previewType</span><span class="sxs-lookup"><span data-stu-id="f368e-134">previewType</span></span>|<span data-ttu-id="f368e-135">string</span><span class="sxs-lookup"><span data-stu-id="f368e-135">string</span></span>|<span data-ttu-id="f368e-p104">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="f368e-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="f368e-139">references</span><span class="sxs-lookup"><span data-stu-id="f368e-139">references</span></span>|[<span data-ttu-id="f368e-140">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="f368e-140">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="f368e-141">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="f368e-141">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f368e-142">关系</span><span class="sxs-lookup"><span data-stu-id="f368e-142">Relationships</span></span>
<span data-ttu-id="f368e-143">无</span><span class="sxs-lookup"><span data-stu-id="f368e-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f368e-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f368e-144">JSON representation</span></span>
<span data-ttu-id="f368e-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f368e-145">Here is a JSON representation of the resource.</span></span>

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
