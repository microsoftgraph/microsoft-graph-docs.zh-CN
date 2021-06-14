---
title: educationFeedback 资源类型
description: 从教师到学生的反馈。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 471c55668e7849f55d5a7623f86bc1f07fc6e537
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912172"
---
# <a name="educationfeedback-resource-type"></a><span data-ttu-id="97ab4-103">educationFeedback 资源类型</span><span class="sxs-lookup"><span data-stu-id="97ab4-103">educationFeedback resource type</span></span>

<span data-ttu-id="97ab4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="97ab4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="97ab4-105">从教师到学生的反馈。</span><span class="sxs-lookup"><span data-stu-id="97ab4-105">Feedback from a teacher to a student.</span></span> 

<span data-ttu-id="97ab4-106">此属性表示反馈的文本部分以及提供反馈的人。</span><span class="sxs-lookup"><span data-stu-id="97ab4-106">This property represents both the text part of the feedback along with who provided the feedback.</span></span>


## <a name="properties"></a><span data-ttu-id="97ab4-107">属性</span><span class="sxs-lookup"><span data-stu-id="97ab4-107">Properties</span></span>
| <span data-ttu-id="97ab4-108">属性</span><span class="sxs-lookup"><span data-stu-id="97ab4-108">Property</span></span>     | <span data-ttu-id="97ab4-109">类型</span><span class="sxs-lookup"><span data-stu-id="97ab4-109">Type</span></span>   |<span data-ttu-id="97ab4-110">说明</span><span class="sxs-lookup"><span data-stu-id="97ab4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97ab4-111">feedbackBy</span><span class="sxs-lookup"><span data-stu-id="97ab4-111">feedbackBy</span></span>|[<span data-ttu-id="97ab4-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="97ab4-112">identitySet</span></span>](identityset.md)|<span data-ttu-id="97ab4-113">创建反馈的用户。</span><span class="sxs-lookup"><span data-stu-id="97ab4-113">User who created the feedback.</span></span>|
|<span data-ttu-id="97ab4-114">feedbackDateTime</span><span class="sxs-lookup"><span data-stu-id="97ab4-114">feedbackDateTime</span></span>|<span data-ttu-id="97ab4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="97ab4-115">DateTimeOffset</span></span>|<span data-ttu-id="97ab4-116">提供反馈的时间。</span><span class="sxs-lookup"><span data-stu-id="97ab4-116">Moment in time when the feedback was given.</span></span> <span data-ttu-id="97ab4-117">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="97ab4-117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="97ab4-118">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="97ab4-118">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="97ab4-119">text</span><span class="sxs-lookup"><span data-stu-id="97ab4-119">text</span></span>|[<span data-ttu-id="97ab4-120">itemBody</span><span class="sxs-lookup"><span data-stu-id="97ab4-120">itemBody</span></span>](itembody.md)|<span data-ttu-id="97ab4-121">反馈。</span><span class="sxs-lookup"><span data-stu-id="97ab4-121">Feedback.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97ab4-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97ab4-122">JSON representation</span></span>

<span data-ttu-id="97ab4-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97ab4-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedback"
}-->

```json
{
  "feedbackBy": {"@odata.type": "microsoft.graph.identitySet"},
  "feedbackDateTime": "String",
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


