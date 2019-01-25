---
title: plannerTaskDetails 资源类型
description: '**plannerTaskDetails** 资源表示任务的其他相关信息。每个任务对象均有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512309"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="1049c-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="1049c-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1049c-p102">**plannerTaskDetails** 资源表示任务的其他相关信息。每个[任务](plannertask.md)对象均有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="1049c-p102">The **plannerTaskDetails** resource represents the additional information about a task. Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="1049c-107">方法</span><span class="sxs-lookup"><span data-stu-id="1049c-107">Methods</span></span>

| <span data-ttu-id="1049c-108">方法</span><span class="sxs-lookup"><span data-stu-id="1049c-108">Method</span></span>           | <span data-ttu-id="1049c-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1049c-109">Return Type</span></span>    |<span data-ttu-id="1049c-110">说明</span><span class="sxs-lookup"><span data-stu-id="1049c-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1049c-111">Get plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="1049c-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="1049c-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="1049c-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="1049c-113">读取 **plannerTaskDetails** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1049c-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="1049c-114">Update</span><span class="sxs-lookup"><span data-stu-id="1049c-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="1049c-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="1049c-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="1049c-116">更新 **plannerTaskDetails** 对象。</span><span class="sxs-lookup"><span data-stu-id="1049c-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1049c-117">属性</span><span class="sxs-lookup"><span data-stu-id="1049c-117">Properties</span></span>
| <span data-ttu-id="1049c-118">属性</span><span class="sxs-lookup"><span data-stu-id="1049c-118">Property</span></span>     | <span data-ttu-id="1049c-119">类型</span><span class="sxs-lookup"><span data-stu-id="1049c-119">Type</span></span>   |<span data-ttu-id="1049c-120">说明</span><span class="sxs-lookup"><span data-stu-id="1049c-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1049c-121">checklist</span><span class="sxs-lookup"><span data-stu-id="1049c-121">checklist</span></span>|[<span data-ttu-id="1049c-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="1049c-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="1049c-123">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="1049c-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="1049c-124">description</span><span class="sxs-lookup"><span data-stu-id="1049c-124">description</span></span>|<span data-ttu-id="1049c-125">String</span><span class="sxs-lookup"><span data-stu-id="1049c-125">String</span></span>|<span data-ttu-id="1049c-126">任务描述</span><span class="sxs-lookup"><span data-stu-id="1049c-126">Description of the task</span></span>|
|<span data-ttu-id="1049c-127">id</span><span class="sxs-lookup"><span data-stu-id="1049c-127">id</span></span>|<span data-ttu-id="1049c-128">String</span><span class="sxs-lookup"><span data-stu-id="1049c-128">String</span></span>| <span data-ttu-id="1049c-129">只读。</span><span class="sxs-lookup"><span data-stu-id="1049c-129">Read-only.</span></span> <span data-ttu-id="1049c-130">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="1049c-130">ID of the task details.</span></span> <span data-ttu-id="1049c-131">它是 28 字符长度和区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1049c-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="1049c-132">服务上执行[格式验证](tasks-identifiers-disclaimer.md)。</span><span class="sxs-lookup"><span data-stu-id="1049c-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="1049c-133">previewType</span><span class="sxs-lookup"><span data-stu-id="1049c-133">previewType</span></span>|<span data-ttu-id="1049c-134">string</span><span class="sxs-lookup"><span data-stu-id="1049c-134">string</span></span>|<span data-ttu-id="1049c-p104">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="1049c-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="1049c-138">references</span><span class="sxs-lookup"><span data-stu-id="1049c-138">references</span></span>|[<span data-ttu-id="1049c-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="1049c-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="1049c-140">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="1049c-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1049c-141">关系</span><span class="sxs-lookup"><span data-stu-id="1049c-141">Relationships</span></span>
<span data-ttu-id="1049c-142">无</span><span class="sxs-lookup"><span data-stu-id="1049c-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1049c-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1049c-143">JSON representation</span></span>
<span data-ttu-id="1049c-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1049c-144">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannertaskdetails.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
