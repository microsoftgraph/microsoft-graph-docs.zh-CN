---
title: plannerTaskDetails 资源类型
description: '**plannerTaskDetails**资源表示有关任务的其他信息。 每个任务对象都有一个详细信息对象。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 579ecdbf43275de90468883d158af725eb1d1734
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563600"
---
# <a name="plannertaskdetails-resource-type"></a><span data-ttu-id="877bd-104">plannerTaskDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="877bd-104">plannerTaskDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="877bd-105">**plannerTaskDetails**资源表示有关任务的其他信息。</span><span class="sxs-lookup"><span data-stu-id="877bd-105">The **plannerTaskDetails** resource represents the additional information about a task.</span></span> <span data-ttu-id="877bd-106">每个[任务](plannertask.md)对象都有一个详细信息对象。</span><span class="sxs-lookup"><span data-stu-id="877bd-106">Each [task](plannertask.md) object has a details object.</span></span>


## <a name="methods"></a><span data-ttu-id="877bd-107">方法</span><span class="sxs-lookup"><span data-stu-id="877bd-107">Methods</span></span>

| <span data-ttu-id="877bd-108">方法</span><span class="sxs-lookup"><span data-stu-id="877bd-108">Method</span></span>           | <span data-ttu-id="877bd-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="877bd-109">Return Type</span></span>    |<span data-ttu-id="877bd-110">说明</span><span class="sxs-lookup"><span data-stu-id="877bd-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="877bd-111">获取 plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="877bd-111">Get plannerTaskDetails</span></span>](../api/plannertaskdetails-get.md) | [<span data-ttu-id="877bd-112">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="877bd-112">plannerTaskDetails</span></span>](plannertaskdetails.md) |<span data-ttu-id="877bd-113">读取**plannerTaskDetails**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="877bd-113">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="877bd-114">更新</span><span class="sxs-lookup"><span data-stu-id="877bd-114">Update</span></span>](../api/plannertaskdetails-update.md) | [<span data-ttu-id="877bd-115">plannerTaskDetails</span><span class="sxs-lookup"><span data-stu-id="877bd-115">plannerTaskDetails</span></span>](plannertaskdetails.md)    |<span data-ttu-id="877bd-116">更新**plannerTaskDetails**对象。</span><span class="sxs-lookup"><span data-stu-id="877bd-116">Update **plannerTaskDetails** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="877bd-117">属性</span><span class="sxs-lookup"><span data-stu-id="877bd-117">Properties</span></span>
| <span data-ttu-id="877bd-118">属性</span><span class="sxs-lookup"><span data-stu-id="877bd-118">Property</span></span>     | <span data-ttu-id="877bd-119">类型</span><span class="sxs-lookup"><span data-stu-id="877bd-119">Type</span></span>   |<span data-ttu-id="877bd-120">说明</span><span class="sxs-lookup"><span data-stu-id="877bd-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="877bd-121">checklist</span><span class="sxs-lookup"><span data-stu-id="877bd-121">checklist</span></span>|[<span data-ttu-id="877bd-122">plannerChecklistItems</span><span class="sxs-lookup"><span data-stu-id="877bd-122">plannerChecklistItems</span></span>](plannerchecklistitems.md)|<span data-ttu-id="877bd-123">任务上的检查表项目集合。</span><span class="sxs-lookup"><span data-stu-id="877bd-123">The collection of checklist items on the task.</span></span>|
|<span data-ttu-id="877bd-124">说明</span><span class="sxs-lookup"><span data-stu-id="877bd-124">description</span></span>|<span data-ttu-id="877bd-125">String</span><span class="sxs-lookup"><span data-stu-id="877bd-125">String</span></span>|<span data-ttu-id="877bd-126">任务描述</span><span class="sxs-lookup"><span data-stu-id="877bd-126">Description of the task</span></span>|
|<span data-ttu-id="877bd-127">id</span><span class="sxs-lookup"><span data-stu-id="877bd-127">id</span></span>|<span data-ttu-id="877bd-128">String</span><span class="sxs-lookup"><span data-stu-id="877bd-128">String</span></span>| <span data-ttu-id="877bd-129">只读。</span><span class="sxs-lookup"><span data-stu-id="877bd-129">Read-only.</span></span> <span data-ttu-id="877bd-130">任务详细信息的 ID。</span><span class="sxs-lookup"><span data-stu-id="877bd-130">ID of the task details.</span></span> <span data-ttu-id="877bd-131">长度为 28 个字符，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="877bd-131">It is 28 characters long and case-sensitive.</span></span> <span data-ttu-id="877bd-132">[格式验证](tasks-identifiers-disclaimer.md)在服务上完成。</span><span class="sxs-lookup"><span data-stu-id="877bd-132">[Format validation](tasks-identifiers-disclaimer.md) is done on the service.</span></span>|
|<span data-ttu-id="877bd-133">previewType</span><span class="sxs-lookup"><span data-stu-id="877bd-133">previewType</span></span>|<span data-ttu-id="877bd-134">string</span><span class="sxs-lookup"><span data-stu-id="877bd-134">string</span></span>|<span data-ttu-id="877bd-p104">这将设置显示在任务上的预览类型。可能的值是：`automatic`、`noPreview`、`checklist`、`description`、`reference`。当设为 `automatic` 时，由查看任务的应用选择显示的预览。</span><span class="sxs-lookup"><span data-stu-id="877bd-p104">This sets the type of preview that shows up on the task. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`. When set to `automatic` the displayed preview is chosen by the app viewing the task.</span></span>|
|<span data-ttu-id="877bd-138">references</span><span class="sxs-lookup"><span data-stu-id="877bd-138">references</span></span>|[<span data-ttu-id="877bd-139">plannerExternalReferences</span><span class="sxs-lookup"><span data-stu-id="877bd-139">plannerExternalReferences</span></span>](plannerexternalreferences.md)|<span data-ttu-id="877bd-140">任务上的引用集合。</span><span class="sxs-lookup"><span data-stu-id="877bd-140">The collection of references on the task.</span></span>|

## <a name="relationships"></a><span data-ttu-id="877bd-141">关系</span><span class="sxs-lookup"><span data-stu-id="877bd-141">Relationships</span></span>
<span data-ttu-id="877bd-142">无</span><span class="sxs-lookup"><span data-stu-id="877bd-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="877bd-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="877bd-143">JSON representation</span></span>
<span data-ttu-id="877bd-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="877bd-144">Here is a JSON representation of the resource.</span></span>

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
