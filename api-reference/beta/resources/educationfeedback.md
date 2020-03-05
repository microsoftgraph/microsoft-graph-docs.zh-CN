---
title: educationFeedback 资源类型
description: 从教师到学生的反馈。 此属性表示反馈的文本部分以及发件人数。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: aac921b1e9f70bc22db2b91833a6b6d348a935db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502142"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="ef54a-104">educationFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef54a-104">educationFeedback resource type</span></span>

<span data-ttu-id="ef54a-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ef54a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef54a-106">从教师到学生的反馈。</span><span class="sxs-lookup"><span data-stu-id="ef54a-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="ef54a-107">此属性表示反馈的文本部分以及发件人数。</span><span class="sxs-lookup"><span data-stu-id="ef54a-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="ef54a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ef54a-108">Properties</span></span>
| <span data-ttu-id="ef54a-109">属性</span><span class="sxs-lookup"><span data-stu-id="ef54a-109">Property</span></span>     | <span data-ttu-id="ef54a-110">类型</span><span class="sxs-lookup"><span data-stu-id="ef54a-110">Type</span></span>   |<span data-ttu-id="ef54a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ef54a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef54a-112">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="ef54a-112">feedbackBy</span></span>|[<span data-ttu-id="ef54a-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="ef54a-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="ef54a-114">创建了反馈的用户。</span><span class="sxs-lookup"><span data-stu-id="ef54a-114">User who created the feedback.</span></span>|
|<span data-ttu-id="ef54a-115">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="ef54a-115">feedbackDateTime</span></span>|<span data-ttu-id="ef54a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef54a-116">DateTimeOffset</span></span>|<span data-ttu-id="ef54a-117">提供反馈的时间点。</span><span class="sxs-lookup"><span data-stu-id="ef54a-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="ef54a-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ef54a-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ef54a-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ef54a-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ef54a-120">text</span><span class="sxs-lookup"><span data-stu-id="ef54a-120">text</span></span>|[<span data-ttu-id="ef54a-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="ef54a-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="ef54a-122">征求.</span><span class="sxs-lookup"><span data-stu-id="ef54a-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef54a-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef54a-123">JSON representation</span></span>

<span data-ttu-id="ef54a-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef54a-124">The following is a JSON representation of the resource.</span></span>

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
