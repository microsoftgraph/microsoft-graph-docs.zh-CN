---
title: educationAssignmentGrade 资源类型
description: " 但是，所有类型的评分 (分数、通过/失败等) 是此类的子类"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 84baeb3a0e3efeee0e5f7e7f6f7d5f6d8f285f59
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722452"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="2bcc8-103">educationAssignmentGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bcc8-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="2bcc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bcc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2bcc8-105">代表 **提交上的 Grade** 对象。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-105">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="2bcc8-106">这是一个永远不会实例化抽象类型;但是，所有类型的评分 (点、通过/失败等) 是此资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="2bcc8-107">此对象还跟踪谁正在评分。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="2bcc8-108">This is used in the **submission.grade** property.</span><span class="sxs-lookup"><span data-stu-id="2bcc8-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="2bcc8-109">属性</span><span class="sxs-lookup"><span data-stu-id="2bcc8-109">Properties</span></span>
| <span data-ttu-id="2bcc8-110">属性</span><span class="sxs-lookup"><span data-stu-id="2bcc8-110">Property</span></span>     | <span data-ttu-id="2bcc8-111">类型</span><span class="sxs-lookup"><span data-stu-id="2bcc8-111">Type</span></span>   |<span data-ttu-id="2bcc8-112">说明</span><span class="sxs-lookup"><span data-stu-id="2bcc8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bcc8-113">gradedBy</span><span class="sxs-lookup"><span data-stu-id="2bcc8-113">gradedBy</span></span>|[<span data-ttu-id="2bcc8-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="2bcc8-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="2bcc8-115">评分的用户。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-115">User who did the grading.</span></span> |
|<span data-ttu-id="2bcc8-116">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="2bcc8-116">gradedDateTime</span></span>|<span data-ttu-id="2bcc8-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2bcc8-117">DateTimeOffset</span></span>| <span data-ttu-id="2bcc8-118">此提交对象应用成绩的时间。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="2bcc8-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2bcc8-120">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2bcc8-120">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bcc8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bcc8-121">JSON representation</span></span>

<span data-ttu-id="2bcc8-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bcc8-122">The following is a JSON representation of the resource.</span></span>

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


