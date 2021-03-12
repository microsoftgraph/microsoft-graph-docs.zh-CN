---
title: plannerExternalReference 资源类型
description: '**plannerExternalReference** 资源表示附件（如文件 (URL）的引用) 。 它是 externalReferences 对象中属性值对的值。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 536e7b6a933ffdad610bf6cce561b2546d60e5d2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722312"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="8f9e5-104">plannerExternalReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="8f9e5-104">plannerExternalReference resource type</span></span>

<span data-ttu-id="8f9e5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8f9e5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8f9e5-106">**plannerExternalReference** 资源表示附件（如文件 (URL）的引用) 。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-106">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL).</span></span> <span data-ttu-id="8f9e5-107">它是 [externalReferences](plannerexternalreferences.md)对象中的属性值对的值。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-107">It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="8f9e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f9e5-108">Properties</span></span>
| <span data-ttu-id="8f9e5-109">属性</span><span class="sxs-lookup"><span data-stu-id="8f9e5-109">Property</span></span>     | <span data-ttu-id="8f9e5-110">类型</span><span class="sxs-lookup"><span data-stu-id="8f9e5-110">Type</span></span>   |<span data-ttu-id="8f9e5-111">说明</span><span class="sxs-lookup"><span data-stu-id="8f9e5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f9e5-112">alias</span><span class="sxs-lookup"><span data-stu-id="8f9e5-112">alias</span></span>|<span data-ttu-id="8f9e5-113">String</span><span class="sxs-lookup"><span data-stu-id="8f9e5-113">String</span></span>|<span data-ttu-id="8f9e5-114">用于描述引用的名称别名。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-114">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="8f9e5-115">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="8f9e5-115">lastModifiedBy</span></span>|[<span data-ttu-id="8f9e5-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="8f9e5-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="8f9e5-117">只读。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-117">Read-only.</span></span> <span data-ttu-id="8f9e5-118">上次修改的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-118">User ID by which this is last modified.</span></span>|
|<span data-ttu-id="8f9e5-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f9e5-119">lastModifiedDateTime</span></span>|<span data-ttu-id="8f9e5-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f9e5-120">DateTimeOffset</span></span>|<span data-ttu-id="8f9e5-121">只读。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-121">Read-only.</span></span> <span data-ttu-id="8f9e5-122">上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-122">Date and time at which this is last modified.</span></span> <span data-ttu-id="8f9e5-123">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8f9e5-124">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="8f9e5-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8f9e5-125">previewPriority</span><span class="sxs-lookup"><span data-stu-id="8f9e5-125">previewPriority</span></span>|<span data-ttu-id="8f9e5-126">字符串</span><span class="sxs-lookup"><span data-stu-id="8f9e5-126">String</span></span>|<span data-ttu-id="8f9e5-127">用于设置引用在任务上显示为预览的相对优先级顺序。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-127">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="8f9e5-128">type</span><span class="sxs-lookup"><span data-stu-id="8f9e5-128">type</span></span>|<span data-ttu-id="8f9e5-129">字符串</span><span class="sxs-lookup"><span data-stu-id="8f9e5-129">String</span></span>|<span data-ttu-id="8f9e5-130">用于描述引用的类型。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-130">Used to describe the type of the reference.</span></span> <span data-ttu-id="8f9e5-131">类型包括 `PowerPoint` `Word` `Excel` ：、、、。 `Other`</span><span class="sxs-lookup"><span data-stu-id="8f9e5-131">Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8f9e5-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8f9e5-132">JSON representation</span></span>
<span data-ttu-id="8f9e5-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f9e5-133">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerExternalReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

