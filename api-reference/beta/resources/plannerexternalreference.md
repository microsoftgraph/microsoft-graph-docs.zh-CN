---
title: plannerExternalReference 资源类型
description: '**PlannerExternalReference**资源表示 （例如文件，URL 附件） 的引用的元数据。 它是 externalReferences 对象中的属性值对的值。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: d484c22d18ffb501cccbd731fa5c3ad4788a8667
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944661"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="d65a1-104">plannerExternalReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="d65a1-104">plannerExternalReference resource type</span></span>

> <span data-ttu-id="d65a1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d65a1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d65a1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d65a1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d65a1-p103">**plannerExternalReference** 资源表示引用（文件、URL 等附件）的元数据。它是 [externalReferences 对象](plannerexternalreferences.md)的属性-值对的值。</span><span class="sxs-lookup"><span data-stu-id="d65a1-p103">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="d65a1-109">属性</span><span class="sxs-lookup"><span data-stu-id="d65a1-109">Properties</span></span>
| <span data-ttu-id="d65a1-110">属性</span><span class="sxs-lookup"><span data-stu-id="d65a1-110">Property</span></span>     | <span data-ttu-id="d65a1-111">类型</span><span class="sxs-lookup"><span data-stu-id="d65a1-111">Type</span></span>   |<span data-ttu-id="d65a1-112">说明</span><span class="sxs-lookup"><span data-stu-id="d65a1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d65a1-113">alias</span><span class="sxs-lookup"><span data-stu-id="d65a1-113">alias</span></span>|<span data-ttu-id="d65a1-114">String</span><span class="sxs-lookup"><span data-stu-id="d65a1-114">String</span></span>|<span data-ttu-id="d65a1-115">描述引用的别名。</span><span class="sxs-lookup"><span data-stu-id="d65a1-115">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="d65a1-116">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="d65a1-116">lastModifiedBy</span></span>|[<span data-ttu-id="d65a1-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="d65a1-117">identitySet</span></span>](identityset.md)|<span data-ttu-id="d65a1-p104">只读。上一次修改它的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="d65a1-p104">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="d65a1-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d65a1-120">lastModifiedDateTime</span></span>|<span data-ttu-id="d65a1-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d65a1-121">DateTimeOffset</span></span>|<span data-ttu-id="d65a1-p105">只读。上一次修改它的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d65a1-p105">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d65a1-126">previewPriority</span><span class="sxs-lookup"><span data-stu-id="d65a1-126">previewPriority</span></span>|<span data-ttu-id="d65a1-127">String</span><span class="sxs-lookup"><span data-stu-id="d65a1-127">String</span></span>|<span data-ttu-id="d65a1-128">用于设置在任务上以预览形式显示引用的相对优先级顺序。</span><span class="sxs-lookup"><span data-stu-id="d65a1-128">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="d65a1-129">type</span><span class="sxs-lookup"><span data-stu-id="d65a1-129">type</span></span>|<span data-ttu-id="d65a1-130">String</span><span class="sxs-lookup"><span data-stu-id="d65a1-130">String</span></span>|<span data-ttu-id="d65a1-p106">用于描述引用的类型。类型包括：`PowerPoint`、`Word`、`Excel`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="d65a1-p106">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d65a1-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d65a1-133">JSON representation</span></span>
<span data-ttu-id="d65a1-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d65a1-134">Here is a JSON representation of the resource.</span></span>

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
