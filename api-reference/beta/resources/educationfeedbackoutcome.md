---
title: educationFeedbackOutcome 资源类型
description: 以文本形式提供反馈的 educationOutcome。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 1c50776f6b8dde27d8f937e8b7ee2028ce1cfca1
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153641"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="9e1d6-103">educationFeedbackOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e1d6-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="9e1d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e1d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e1d6-105">表示对 [文本形式的 educationOutcome](educationoutcome.md) 对象的反馈。</span><span class="sxs-lookup"><span data-stu-id="9e1d6-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="9e1d6-106">方法</span><span class="sxs-lookup"><span data-stu-id="9e1d6-106">Methods</span></span>

| <span data-ttu-id="9e1d6-107">方法</span><span class="sxs-lookup"><span data-stu-id="9e1d6-107">Method</span></span>       | <span data-ttu-id="9e1d6-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="9e1d6-108">Return Type</span></span> | <span data-ttu-id="9e1d6-109">说明</span><span class="sxs-lookup"><span data-stu-id="9e1d6-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9e1d6-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="9e1d6-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="9e1d6-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="9e1d6-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="9e1d6-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="9e1d6-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9e1d6-113">属性</span><span class="sxs-lookup"><span data-stu-id="9e1d6-113">Properties</span></span>

| <span data-ttu-id="9e1d6-114">属性</span><span class="sxs-lookup"><span data-stu-id="9e1d6-114">Property</span></span>     | <span data-ttu-id="9e1d6-115">类型</span><span class="sxs-lookup"><span data-stu-id="9e1d6-115">Type</span></span>        | <span data-ttu-id="9e1d6-116">说明</span><span class="sxs-lookup"><span data-stu-id="9e1d6-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9e1d6-117">反馈</span><span class="sxs-lookup"><span data-stu-id="9e1d6-117">feedback</span></span>|[<span data-ttu-id="9e1d6-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="9e1d6-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="9e1d6-119">教师向学生提供的反馈。</span><span class="sxs-lookup"><span data-stu-id="9e1d6-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="9e1d6-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="9e1d6-120">publishedFeedback</span></span>|[<span data-ttu-id="9e1d6-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="9e1d6-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="9e1d6-122">在将成绩发布给学生时进行的反馈属性的副本。</span><span class="sxs-lookup"><span data-stu-id="9e1d6-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e1d6-123">关系</span><span class="sxs-lookup"><span data-stu-id="9e1d6-123">Relationships</span></span>

<span data-ttu-id="9e1d6-124">无</span><span class="sxs-lookup"><span data-stu-id="9e1d6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e1d6-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e1d6-125">JSON representation</span></span>

<span data-ttu-id="9e1d6-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e1d6-126">The following is a JSON representation of the resource.</span></span>

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

