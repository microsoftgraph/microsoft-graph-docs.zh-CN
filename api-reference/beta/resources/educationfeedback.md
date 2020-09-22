---
title: educationFeedback 资源类型
description: 从教师到学生的反馈。 此属性表示反馈的文本部分以及发件人数。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 00514ce99860fa52d167465fb223dad2981c28db
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095476"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="1f9de-104">educationFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="1f9de-104">educationFeedback resource type</span></span>

<span data-ttu-id="1f9de-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f9de-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f9de-106">从教师到学生的反馈。</span><span class="sxs-lookup"><span data-stu-id="1f9de-106">Feedback from a teacher to a student.</span></span> <span data-ttu-id="1f9de-107">此属性表示反馈的文本部分以及发件人数。</span><span class="sxs-lookup"><span data-stu-id="1f9de-107">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="1f9de-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f9de-108">Properties</span></span>
| <span data-ttu-id="1f9de-109">属性</span><span class="sxs-lookup"><span data-stu-id="1f9de-109">Property</span></span>     | <span data-ttu-id="1f9de-110">类型</span><span class="sxs-lookup"><span data-stu-id="1f9de-110">Type</span></span>   |<span data-ttu-id="1f9de-111">说明</span><span class="sxs-lookup"><span data-stu-id="1f9de-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f9de-112">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="1f9de-112">feedbackBy</span></span>|[<span data-ttu-id="1f9de-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="1f9de-113">identitySet</span></span>](identityset.md)|<span data-ttu-id="1f9de-114">创建了反馈的用户。</span><span class="sxs-lookup"><span data-stu-id="1f9de-114">User who created the feedback.</span></span>|
|<span data-ttu-id="1f9de-115">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="1f9de-115">feedbackDateTime</span></span>|<span data-ttu-id="1f9de-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1f9de-116">DateTimeOffset</span></span>|<span data-ttu-id="1f9de-117">提供反馈的时间点。</span><span class="sxs-lookup"><span data-stu-id="1f9de-117">Moment in time when the feedback was given.</span></span> <span data-ttu-id="1f9de-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="1f9de-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1f9de-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="1f9de-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="1f9de-120">text</span><span class="sxs-lookup"><span data-stu-id="1f9de-120">text</span></span>|[<span data-ttu-id="1f9de-121">itemBody</span><span class="sxs-lookup"><span data-stu-id="1f9de-121">itemBody</span></span>](itembody.md)|<span data-ttu-id="1f9de-122">征求.</span><span class="sxs-lookup"><span data-stu-id="1f9de-122">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1f9de-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1f9de-123">JSON representation</span></span>

<span data-ttu-id="1f9de-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f9de-124">The following is a JSON representation of the resource.</span></span>

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


