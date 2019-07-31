---
title: plannerExternalReference 资源类型
description: '**PlannerExternalReference**资源表示引用的元数据 (如文件、URL)。 它是 externalReferences 对象中的属性-值对的值。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 2ac2b6bef3f2e4e24bfc6e789536f4952d89bb6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965999"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="4d3ed-104">plannerExternalReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d3ed-104">plannerExternalReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d3ed-105">**PlannerExternalReference**资源表示引用的元数据 (如文件、URL)。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-105">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="4d3ed-106">它是[externalReferences 对象](plannerexternalreferences.md)中的属性-值对的值。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-106">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="4d3ed-107">属性</span><span class="sxs-lookup"><span data-stu-id="4d3ed-107">Properties</span></span>
| <span data-ttu-id="4d3ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="4d3ed-108">Property</span></span>     | <span data-ttu-id="4d3ed-109">类型</span><span class="sxs-lookup"><span data-stu-id="4d3ed-109">Type</span></span>   |<span data-ttu-id="4d3ed-110">说明</span><span class="sxs-lookup"><span data-stu-id="4d3ed-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4d3ed-111">alias</span><span class="sxs-lookup"><span data-stu-id="4d3ed-111">alias</span></span>|<span data-ttu-id="4d3ed-112">String</span><span class="sxs-lookup"><span data-stu-id="4d3ed-112">String</span></span>|<span data-ttu-id="4d3ed-113">用于描述引用的名称别名。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="4d3ed-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="4d3ed-114">lastModifiedBy</span></span>|[<span data-ttu-id="4d3ed-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="4d3ed-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="4d3ed-116">只读。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-116">Read-only.</span></span> <span data-ttu-id="4d3ed-117">上次修改此 ID 的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-117">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="4d3ed-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4d3ed-118">lastModifiedDateTime</span></span>|<span data-ttu-id="4d3ed-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4d3ed-119">DateTimeOffset</span></span>|<span data-ttu-id="4d3ed-120">只读。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-120">Read-only.</span></span> <span data-ttu-id="4d3ed-121">上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-121">Date and time at which this is last modified.</span></span> <span data-ttu-id="4d3ed-122">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4d3ed-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4d3ed-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4d3ed-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="4d3ed-124">previewPriority</span></span>|<span data-ttu-id="4d3ed-125">String</span><span class="sxs-lookup"><span data-stu-id="4d3ed-125">String</span></span>|<span data-ttu-id="4d3ed-126">用于设置引用将显示为任务预览的相对优先级顺序。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="4d3ed-127">type</span><span class="sxs-lookup"><span data-stu-id="4d3ed-127">type</span></span>|<span data-ttu-id="4d3ed-128">String</span><span class="sxs-lookup"><span data-stu-id="4d3ed-128">String</span></span>|<span data-ttu-id="4d3ed-129">用于描述引用的类型。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-129">Used to describe the type of the reference.</span></span> <span data-ttu-id="4d3ed-130">类型包括: `PowerPoint`、 `Word`、 `Excel`、 `Other`。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-130">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d3ed-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d3ed-131">JSON representation</span></span>
<span data-ttu-id="4d3ed-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d3ed-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerExternalReference"
}-->

```json
{
  "alias": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)",
  "previewPriority": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
