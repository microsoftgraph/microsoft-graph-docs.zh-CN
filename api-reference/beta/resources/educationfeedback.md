---
title: educationFeedback 资源类型
description: 从教师向学生的反馈。 此属性表示以及 who 反馈这两个的文本部分。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 0d08f3bc5c7b4882693cdcbba41b364734c6ccef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873561"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="a6695-104">educationFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6695-104">educationFeedback resource type</span></span>

> <span data-ttu-id="a6695-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a6695-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a6695-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a6695-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a6695-107">从教师向学生的反馈。</span><span class="sxs-lookup"><span data-stu-id="a6695-107">Feedback from a teacher to a student.</span></span> <span data-ttu-id="a6695-108">此属性表示以及 who 反馈这两个的文本部分。</span><span class="sxs-lookup"><span data-stu-id="a6695-108">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="a6695-109">属性</span><span class="sxs-lookup"><span data-stu-id="a6695-109">Properties</span></span>
| <span data-ttu-id="a6695-110">属性</span><span class="sxs-lookup"><span data-stu-id="a6695-110">Property</span></span>     | <span data-ttu-id="a6695-111">类型</span><span class="sxs-lookup"><span data-stu-id="a6695-111">Type</span></span>   |<span data-ttu-id="a6695-112">Description</span><span class="sxs-lookup"><span data-stu-id="a6695-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6695-113">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="a6695-113">feedbackBy</span></span>|[<span data-ttu-id="a6695-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="a6695-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="a6695-115">创建用户的反馈。</span><span class="sxs-lookup"><span data-stu-id="a6695-115">User who created the feedback.</span></span>|
|<span data-ttu-id="a6695-116">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="a6695-116">feedbackDateTime</span></span>|<span data-ttu-id="a6695-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6695-117">DateTimeOffset</span></span>|<span data-ttu-id="a6695-118">提供反馈时时刻。</span><span class="sxs-lookup"><span data-stu-id="a6695-118">Moment in time when the feedback was given.</span></span> <span data-ttu-id="a6695-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="a6695-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a6695-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="a6695-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a6695-121">text</span><span class="sxs-lookup"><span data-stu-id="a6695-121">text</span></span>|[<span data-ttu-id="a6695-122">itemBody</span><span class="sxs-lookup"><span data-stu-id="a6695-122">itemBody</span></span>](itembody.md)|<span data-ttu-id="a6695-123">反馈。</span><span class="sxs-lookup"><span data-stu-id="a6695-123">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6695-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6695-124">JSON representation</span></span>

<span data-ttu-id="a6695-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6695-125">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedback resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
