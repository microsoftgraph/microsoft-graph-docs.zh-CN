---
title: educationFeedback 资源类型
description: 从教师到学生的反馈。 此属性表示反馈的文本部分以及发件人数。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 7ef923870d94479d7ea1d9d762ee729b5060afd6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340506"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="c55c5-104">educationFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="c55c5-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c55c5-105">从教师到学生的反馈。</span><span class="sxs-lookup"><span data-stu-id="c55c5-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="c55c5-106">此属性表示反馈的文本部分以及发件人数。</span><span class="sxs-lookup"><span data-stu-id="c55c5-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="c55c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="c55c5-107">Properties</span></span>
| <span data-ttu-id="c55c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="c55c5-108">Property</span></span>     | <span data-ttu-id="c55c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="c55c5-109">Type</span></span>   |<span data-ttu-id="c55c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="c55c5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c55c5-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="c55c5-111">feedbackBy</span></span>|[<span data-ttu-id="c55c5-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="c55c5-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="c55c5-113">创建了反馈的用户。</span><span class="sxs-lookup"><span data-stu-id="c55c5-113">User who created the feedback.</span></span>|
|<span data-ttu-id="c55c5-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="c55c5-114">feedbackDateTime</span></span>|<span data-ttu-id="c55c5-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c55c5-115">DateTimeOffset</span></span>|<span data-ttu-id="c55c5-116">提供反馈的时间点。</span><span class="sxs-lookup"><span data-stu-id="c55c5-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="c55c5-117">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c55c5-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c55c5-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c55c5-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c55c5-119">text</span><span class="sxs-lookup"><span data-stu-id="c55c5-119">text</span></span>|[<span data-ttu-id="c55c5-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="c55c5-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="c55c5-121">征求.</span><span class="sxs-lookup"><span data-stu-id="c55c5-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c55c5-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c55c5-122">JSON representation</span></span>

<span data-ttu-id="c55c5-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c55c5-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String (timestamp)",
  "text": {"@odata.type": "microsoft.graph.itemBody"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
