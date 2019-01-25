---
title: educationAssignmentGrade 资源类型
description: " 但是，所有类型的分级 （磅、 通过/失败，等等） 都是此的子类"
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 5ca13ba057ef000a468d910d49288d9ae8e0c962
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527855"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="99536-103">educationAssignmentGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="99536-103">educationAssignmentGrade resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99536-104">表示在提交的**薪等级**对象。</span><span class="sxs-lookup"><span data-stu-id="99536-104">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="99536-105">这是一个抽象类型，绝不会实例化;但是，所有类型的分级 （磅、 通过/失败，等等） 都是此资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="99536-105">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="99536-106">此对象还会跟踪谁在做分级。</span><span class="sxs-lookup"><span data-stu-id="99536-106">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="99536-107">这使用**submission.grade**属性中。</span><span class="sxs-lookup"><span data-stu-id="99536-107">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="99536-108">属性</span><span class="sxs-lookup"><span data-stu-id="99536-108">Properties</span></span>
| <span data-ttu-id="99536-109">属性</span><span class="sxs-lookup"><span data-stu-id="99536-109">Property</span></span>     | <span data-ttu-id="99536-110">类型</span><span class="sxs-lookup"><span data-stu-id="99536-110">Type</span></span>   |<span data-ttu-id="99536-111">说明</span><span class="sxs-lookup"><span data-stu-id="99536-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99536-112">gradedBy</span><span class="sxs-lookup"><span data-stu-id="99536-112">gradedBy</span></span>|[<span data-ttu-id="99536-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="99536-113">identitySet</span></span>](identityset.md)| <span data-ttu-id="99536-114">未评分的用户。</span><span class="sxs-lookup"><span data-stu-id="99536-114">User who did the grading.</span></span> |
|<span data-ttu-id="99536-115">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="99536-115">gradedDateTime</span></span>|<span data-ttu-id="99536-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99536-116">DateTimeOffset</span></span>| <span data-ttu-id="99536-117">当薪等级已应用于此提交对象时刻。</span><span class="sxs-lookup"><span data-stu-id="99536-117">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="99536-118">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="99536-118">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="99536-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99536-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99536-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99536-120">JSON representation</span></span>

<span data-ttu-id="99536-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99536-121">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentgrade.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
