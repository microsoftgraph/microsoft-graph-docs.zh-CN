---
title: educationAssignmentGrade 资源类型
description: " 但是，所有类型的评分（点、pass/fail 等）都是此类的子类"
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9680a298c405a81648ba0a5fe95cdf0df0c841bb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502744"
---
# <a name="educationassignmentgrade-resource-type"></a><span data-ttu-id="eb5ac-103">educationAssignmentGrade 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb5ac-103">educationAssignmentGrade resource type</span></span>

<span data-ttu-id="eb5ac-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="eb5ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb5ac-105">代表提交中的**年级**对象。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-105">Represents the **Grade** object on a Submission.</span></span> <span data-ttu-id="eb5ac-106">这是一个永远不会实例化的抽象类型;但是，所有类型的评分（点、pass/fail 等）都是此资源类型的子类。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-106">This is an abstract type that will never be instantiated; however, all types of grading (points, pass/fail, and so on) are subclasses of this resource type.</span></span> <span data-ttu-id="eb5ac-107">此对象还跟踪正在进行评分的团队。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-107">This object also tracks who is doing the grading.</span></span> <span data-ttu-id="eb5ac-108">这在**提交. 年级**属性中使用。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-108">This is used in the **submission.grade** property.</span></span>


## <a name="properties"></a><span data-ttu-id="eb5ac-109">属性</span><span class="sxs-lookup"><span data-stu-id="eb5ac-109">Properties</span></span>
| <span data-ttu-id="eb5ac-110">属性</span><span class="sxs-lookup"><span data-stu-id="eb5ac-110">Property</span></span>     | <span data-ttu-id="eb5ac-111">类型</span><span class="sxs-lookup"><span data-stu-id="eb5ac-111">Type</span></span>   |<span data-ttu-id="eb5ac-112">说明</span><span class="sxs-lookup"><span data-stu-id="eb5ac-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb5ac-113">gradedBy</span><span class="sxs-lookup"><span data-stu-id="eb5ac-113">gradedBy</span></span>|[<span data-ttu-id="eb5ac-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="eb5ac-114">identitySet</span></span>](identityset.md)| <span data-ttu-id="eb5ac-115">执行评分的用户。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-115">User who did the grading.</span></span> |
|<span data-ttu-id="eb5ac-116">gradedDateTime</span><span class="sxs-lookup"><span data-stu-id="eb5ac-116">gradedDateTime</span></span>|<span data-ttu-id="eb5ac-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eb5ac-117">DateTimeOffset</span></span>| <span data-ttu-id="eb5ac-118">将评分应用于此提交对象的时间点。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-118">Moment in time when the grade was applied to this submission object.</span></span> <span data-ttu-id="eb5ac-119">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-119">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="eb5ac-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="eb5ac-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb5ac-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb5ac-121">JSON representation</span></span>

<span data-ttu-id="eb5ac-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb5ac-122">The following is a JSON representation of the resource.</span></span>

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
