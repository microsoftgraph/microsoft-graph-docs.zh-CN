---
title: plannerExternalReference 资源类型
description: '**PlannerExternalReference**资源表示引用的元数据（如文件、URL）。 它是 externalReferences 对象中的属性-值对的值。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 04ea5aa373cc0828386f56b8ec80b07faef40f06
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521753"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="0d739-104">plannerExternalReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d739-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="0d739-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0d739-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0d739-106">**PlannerExternalReference**资源表示引用的元数据（如文件、URL）。</span><span class="sxs-lookup"><span data-stu-id="0d739-106">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="0d739-107">它是[externalReferences 对象](plannerexternalreferences.md)中的属性-值对的值。</span><span class="sxs-lookup"><span data-stu-id="0d739-107">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="0d739-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d739-108">Properties</span></span>
| <span data-ttu-id="0d739-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d739-109">Property</span></span>     | <span data-ttu-id="0d739-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d739-110">Type</span></span>   |<span data-ttu-id="0d739-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d739-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d739-112">alias</span><span class="sxs-lookup"><span data-stu-id="0d739-112">alias</span></span>|<span data-ttu-id="0d739-113">String</span><span class="sxs-lookup"><span data-stu-id="0d739-113">String</span></span>|<span data-ttu-id="0d739-114">用于描述引用的名称别名。</span><span class="sxs-lookup"><span data-stu-id="0d739-114">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="0d739-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="0d739-115">lastModifiedBy</span></span>|[<span data-ttu-id="0d739-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="0d739-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="0d739-117">只读。</span><span class="sxs-lookup"><span data-stu-id="0d739-117">Read-only.</span></span> <span data-ttu-id="0d739-118">上次修改此 ID 的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="0d739-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="0d739-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0d739-119">lastModifiedDateTime</span></span>|<span data-ttu-id="0d739-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0d739-120">DateTimeOffset</span></span>|<span data-ttu-id="0d739-121">只读。</span><span class="sxs-lookup"><span data-stu-id="0d739-121">Read-only.</span></span> <span data-ttu-id="0d739-122">上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="0d739-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="0d739-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="0d739-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0d739-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0d739-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0d739-125">previewPriority</span><span class="sxs-lookup"><span data-stu-id="0d739-125">previewPriority</span></span>|<span data-ttu-id="0d739-126">String</span><span class="sxs-lookup"><span data-stu-id="0d739-126">String</span></span>|<span data-ttu-id="0d739-127">用于设置引用将显示为任务预览的相对优先级顺序。</span><span class="sxs-lookup"><span data-stu-id="0d739-127">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="0d739-128">type</span><span class="sxs-lookup"><span data-stu-id="0d739-128">type</span></span>|<span data-ttu-id="0d739-129">String</span><span class="sxs-lookup"><span data-stu-id="0d739-129">String</span></span>|<span data-ttu-id="0d739-130">用于描述引用的类型。</span><span class="sxs-lookup"><span data-stu-id="0d739-130">Used to describe the type of the reference.</span></span> <span data-ttu-id="0d739-131">类型包括： `PowerPoint`、 `Word`、 `Excel`、 `Other`。</span><span class="sxs-lookup"><span data-stu-id="0d739-131">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0d739-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d739-132">JSON representation</span></span>
<span data-ttu-id="0d739-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d739-133">Here is a JSON representation of the resource.</span></span>

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
