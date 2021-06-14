---
title: educationFeedbackOutcome 资源类型
description: 以文本形式提供反馈的 educationOutcome。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d29a09ccca331e466812c44e8f397696d1eb3539
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912243"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="23706-103">educationFeedbackOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="23706-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="23706-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23706-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="23706-105">表示对 [文本形式的 educationOutcome](educationoutcome.md) 对象的反馈。</span><span class="sxs-lookup"><span data-stu-id="23706-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="23706-106">方法</span><span class="sxs-lookup"><span data-stu-id="23706-106">Methods</span></span>

| <span data-ttu-id="23706-107">方法</span><span class="sxs-lookup"><span data-stu-id="23706-107">Method</span></span>       | <span data-ttu-id="23706-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="23706-108">Return Type</span></span> | <span data-ttu-id="23706-109">说明</span><span class="sxs-lookup"><span data-stu-id="23706-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="23706-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="23706-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="23706-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="23706-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="23706-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="23706-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="23706-113">属性</span><span class="sxs-lookup"><span data-stu-id="23706-113">Properties</span></span>

| <span data-ttu-id="23706-114">属性</span><span class="sxs-lookup"><span data-stu-id="23706-114">Property</span></span>     | <span data-ttu-id="23706-115">类型</span><span class="sxs-lookup"><span data-stu-id="23706-115">Type</span></span>        | <span data-ttu-id="23706-116">说明</span><span class="sxs-lookup"><span data-stu-id="23706-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="23706-117">反馈</span><span class="sxs-lookup"><span data-stu-id="23706-117">feedback</span></span>|[<span data-ttu-id="23706-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="23706-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="23706-119">教师向学生提供书面反馈。</span><span class="sxs-lookup"><span data-stu-id="23706-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="23706-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="23706-120">publishedFeedback</span></span>|[<span data-ttu-id="23706-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="23706-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="23706-122">在将成绩发布给学生时所创建的反馈属性的副本。</span><span class="sxs-lookup"><span data-stu-id="23706-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23706-123">关系</span><span class="sxs-lookup"><span data-stu-id="23706-123">Relationships</span></span>

<span data-ttu-id="23706-124">无</span><span class="sxs-lookup"><span data-stu-id="23706-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23706-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="23706-125">JSON representation</span></span>

<span data-ttu-id="23706-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="23706-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "keyProperty": "id"
}-->

```json
{
  "feedback": {"@odata.type": "microsoft.graph.educationFeedback"},
  "publishedFeedback": {"@odata.type": "microsoft.graph.educationFeedback"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationFeedbackOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

