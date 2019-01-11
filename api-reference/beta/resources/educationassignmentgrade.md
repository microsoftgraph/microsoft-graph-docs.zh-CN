---
title: educationAssignmentGrade 资源类型
description: " 但是，所有类型的分级 （磅、 通过/失败，等等） 都是此的子类"
localization_priority: Normal
ms.openlocfilehash: 371346c6ff23623a118b9ee169e563e75e2429f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889010"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="fddc1-103">educationAssignmentGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="fddc1-103">educationAssignmentGrade resource type</span></span>

> <span data-ttu-id="fddc1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fddc1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fddc1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fddc1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fddc1-106">表示在提交的**薪等级**对象。</span><span class="sxs-lookup"><span data-stu-id="fddc1-106">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="fddc1-107">这是一个抽象类型，绝不会实例化;但是，所有类型的分级 （磅、 通过/失败，等等） 都是此资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="fddc1-107">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="fddc1-108">此对象还会跟踪谁在做分级。</span><span class="sxs-lookup"><span data-stu-id="fddc1-108">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="fddc1-109">这使用**submission.grade**属性中。</span><span class="sxs-lookup"><span data-stu-id="fddc1-109">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="fddc1-110">属性</span><span class="sxs-lookup"><span data-stu-id="fddc1-110">Properties</span></span>
| <span data-ttu-id="fddc1-111">属性</span><span class="sxs-lookup"><span data-stu-id="fddc1-111">Property</span></span>     | <span data-ttu-id="fddc1-112">类型</span><span class="sxs-lookup"><span data-stu-id="fddc1-112">Type</span></span>   |<span data-ttu-id="fddc1-113">Description</span><span class="sxs-lookup"><span data-stu-id="fddc1-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fddc1-114">gradedBy</span><span class="sxs-lookup"><span data-stu-id="fddc1-114">gradedBy</span></span>|[<span data-ttu-id="fddc1-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="fddc1-115">identitySet</span></span>](identityset.md)| <span data-ttu-id="fddc1-116">未评分的用户。</span><span class="sxs-lookup"><span data-stu-id="fddc1-116">User who did the grading.</span></span> |
|<span data-ttu-id="fddc1-117">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="fddc1-117">gradedDateTime</span></span>|<span data-ttu-id="fddc1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fddc1-118">DateTimeOffset</span></span>| <span data-ttu-id="fddc1-119">当薪等级已应用于此提交对象时刻。</span><span class="sxs-lookup"><span data-stu-id="fddc1-119">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="fddc1-120">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fddc1-120">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fddc1-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="fddc1-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fddc1-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fddc1-122">JSON representation</span></span>

<span data-ttu-id="fddc1-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fddc1-123">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentGrade resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
