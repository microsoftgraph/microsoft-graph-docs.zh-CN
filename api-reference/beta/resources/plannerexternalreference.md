---
title: plannerExternalReference 资源类型
description: '**plannerExternalReference** 资源表示引用（文件、URL 等附件）的元数据。它是 externalReferences 对象的属性-值对的值。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: 95084e8a4d2d1b117fc627902b2bd8163fcc82f6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518707"
---
# <a name="plannerexternalreference-resource-type"></a><span data-ttu-id="cf79b-104">plannerExternalReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf79b-104">plannerExternalReference resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf79b-p102">**plannerExternalReference** 资源表示引用（文件、URL 等附件）的元数据。它是 [externalReferences 对象](plannerexternalreferences.md)的属性-值对的值。</span><span class="sxs-lookup"><span data-stu-id="cf79b-p102">The **plannerExternalReference** resource represents the metadata of a reference (attachments such as file, URL). It is the value of property-value pairs in the [externalReferences object](plannerexternalreferences.md).</span></span>



## <a name="properties"></a><span data-ttu-id="cf79b-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf79b-107">Properties</span></span>
| <span data-ttu-id="cf79b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf79b-108">Property</span></span>     | <span data-ttu-id="cf79b-109">类型</span><span class="sxs-lookup"><span data-stu-id="cf79b-109">Type</span></span>   |<span data-ttu-id="cf79b-110">说明</span><span class="sxs-lookup"><span data-stu-id="cf79b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf79b-111">alias</span><span class="sxs-lookup"><span data-stu-id="cf79b-111">alias</span></span>|<span data-ttu-id="cf79b-112">String</span><span class="sxs-lookup"><span data-stu-id="cf79b-112">String</span></span>|<span data-ttu-id="cf79b-113">描述引用的别名。</span><span class="sxs-lookup"><span data-stu-id="cf79b-113">A name alias to describe the reference.</span></span>|
|<span data-ttu-id="cf79b-114">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="cf79b-114">lastModifiedBy</span></span>|[<span data-ttu-id="cf79b-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="cf79b-115">identitySet</span></span>](identityset.md)|<span data-ttu-id="cf79b-p103">只读。上一次修改它的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="cf79b-p103">Read-only. User ID by which this is last modified.</span></span>|
|<span data-ttu-id="cf79b-118">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cf79b-118">lastModifiedDateTime</span></span>|<span data-ttu-id="cf79b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf79b-119">DateTimeOffset</span></span>|<span data-ttu-id="cf79b-p104">只读。上一次修改它的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="cf79b-p104">Read-only. Date and time at which this is last modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="cf79b-124">previewPriority</span><span class="sxs-lookup"><span data-stu-id="cf79b-124">previewPriority</span></span>|<span data-ttu-id="cf79b-125">String</span><span class="sxs-lookup"><span data-stu-id="cf79b-125">String</span></span>|<span data-ttu-id="cf79b-126">用于设置在任务上以预览形式显示引用的相对优先级顺序。</span><span class="sxs-lookup"><span data-stu-id="cf79b-126">Used to set the relative priority order in which the reference will be shown as a preview on the task.</span></span>|
|<span data-ttu-id="cf79b-127">type</span><span class="sxs-lookup"><span data-stu-id="cf79b-127">type</span></span>|<span data-ttu-id="cf79b-128">String</span><span class="sxs-lookup"><span data-stu-id="cf79b-128">String</span></span>|<span data-ttu-id="cf79b-p105">用于描述引用的类型。类型包括：`PowerPoint`、`Word`、`Excel`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="cf79b-p105">Used to describe the type of the reference. Types include: `PowerPoint`, `Word`, `Excel`, `Other`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf79b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf79b-131">JSON representation</span></span>
<span data-ttu-id="cf79b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf79b-132">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerexternalreference.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
