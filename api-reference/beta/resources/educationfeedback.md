---
title: educationFeedback 资源类型
description: 从教师向学生的反馈。 此属性表示以及 who 反馈这两个的文本部分。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 90e55b20b371d04bc3c6d45bb84fe6bf42157a2f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515634"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="aa332-104">educationFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa332-104">educationFeedback resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa332-105">从教师向学生的反馈。</span><span class="sxs-lookup"><span data-stu-id="aa332-105">Feedback from a teacher to a student.</span></span> <span data-ttu-id="aa332-106">此属性表示以及 who 反馈这两个的文本部分。</span><span class="sxs-lookup"><span data-stu-id="aa332-106">This property represents both the text part of the feedback along with the who.</span></span>


## <a name="properties"></a><span data-ttu-id="aa332-107">属性</span><span class="sxs-lookup"><span data-stu-id="aa332-107">Properties</span></span>
| <span data-ttu-id="aa332-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa332-108">Property</span></span>     | <span data-ttu-id="aa332-109">类型</span><span class="sxs-lookup"><span data-stu-id="aa332-109">Type</span></span>   |<span data-ttu-id="aa332-110">说明</span><span class="sxs-lookup"><span data-stu-id="aa332-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa332-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="aa332-111">feedbackBy</span></span>|[<span data-ttu-id="aa332-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="aa332-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="aa332-113">创建用户的反馈。</span><span class="sxs-lookup"><span data-stu-id="aa332-113">User who created the feedback.</span></span>|
|<span data-ttu-id="aa332-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="aa332-114">feedbackDateTime</span></span>|<span data-ttu-id="aa332-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa332-115">DateTimeOffset</span></span>|<span data-ttu-id="aa332-116">提供反馈时时刻。</span><span class="sxs-lookup"><span data-stu-id="aa332-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="aa332-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="aa332-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aa332-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="aa332-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="aa332-119">text</span><span class="sxs-lookup"><span data-stu-id="aa332-119">text</span></span>|[<span data-ttu-id="aa332-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="aa332-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="aa332-121">反馈</span><span class="sxs-lookup"><span data-stu-id="aa332-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa332-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa332-122">JSON representation</span></span>

<span data-ttu-id="aa332-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa332-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfeedback.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
