---
title: educationAssignmentGrade 资源类型
description: " 但是, 所有类型的评分 (点、pass/fail 等) 都是此类的子类"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: e925059a5eb06e5cc9795f78368b884fa40dd3ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334533"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="f0292-103">educationAssignmentGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0292-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0292-104">代表提交中的**年级**对象。</span><span class="sxs-lookup"><span data-stu-id="f0292-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="f0292-105">这是一个永远不会实例化的抽象类型;但是, 所有类型的评分 (点、pass/fail 等) 都是此资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="f0292-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="f0292-106">此对象还跟踪正在进行评分的团队。</span><span class="sxs-lookup"><span data-stu-id="f0292-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="f0292-107">这在**提交. 年级**属性中使用。</span><span class="sxs-lookup"><span data-stu-id="f0292-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="f0292-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0292-108">Properties</span></span>
| <span data-ttu-id="f0292-109">属性</span><span class="sxs-lookup"><span data-stu-id="f0292-109">Property</span></span>     | <span data-ttu-id="f0292-110">类型</span><span class="sxs-lookup"><span data-stu-id="f0292-110">Type</span></span>   |<span data-ttu-id="f0292-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0292-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0292-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="f0292-112">gradedBy</span></span>|[<span data-ttu-id="f0292-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="f0292-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="f0292-114">执行评分的用户。</span><span class="sxs-lookup"><span data-stu-id="f0292-114">User who did the grading.</span></span> |
|<span data-ttu-id="f0292-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0292-115">gradedDateTime</span></span>|<span data-ttu-id="f0292-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0292-116">DateTimeOffset</span></span>| <span data-ttu-id="f0292-117">将评分应用于此提交对象的时间点。</span><span class="sxs-lookup"><span data-stu-id="f0292-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="f0292-118">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f0292-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f0292-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f0292-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0292-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0292-120">JSON representation</span></span>

<span data-ttu-id="f0292-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0292-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}-->

```json
{
  "gradedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "gradedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
