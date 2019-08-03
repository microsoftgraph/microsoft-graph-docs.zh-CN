---
title: educationFeedbackOutcome 资源类型
description: 以文本形式提供反馈的 educationOutcome。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e61538a62a1bb267b0a13b98b17e9b69a8ceed92
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173249"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="44a39-103">educationFeedbackOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="44a39-103">educationFeedbackOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="44a39-104">以文本形式表示对[educationOutcome](educationoutcome.md)对象的反馈。</span><span class="sxs-lookup"><span data-stu-id="44a39-104">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="44a39-105">方法</span><span class="sxs-lookup"><span data-stu-id="44a39-105">Methods</span></span>

| <span data-ttu-id="44a39-106">方法</span><span class="sxs-lookup"><span data-stu-id="44a39-106">Method</span></span>       | <span data-ttu-id="44a39-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="44a39-107">Return Type</span></span> | <span data-ttu-id="44a39-108">说明</span><span class="sxs-lookup"><span data-stu-id="44a39-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="44a39-109">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="44a39-109">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="44a39-110">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="44a39-110">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="44a39-111">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="44a39-111">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="44a39-112">属性</span><span class="sxs-lookup"><span data-stu-id="44a39-112">Properties</span></span>

| <span data-ttu-id="44a39-113">属性</span><span class="sxs-lookup"><span data-stu-id="44a39-113">Property</span></span>     | <span data-ttu-id="44a39-114">类型</span><span class="sxs-lookup"><span data-stu-id="44a39-114">Type</span></span>        | <span data-ttu-id="44a39-115">说明</span><span class="sxs-lookup"><span data-stu-id="44a39-115">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="44a39-116">反馈</span><span class="sxs-lookup"><span data-stu-id="44a39-116">feedback</span></span>|[<span data-ttu-id="44a39-117">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="44a39-117">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="44a39-118">教师对学生的书面反馈。</span><span class="sxs-lookup"><span data-stu-id="44a39-118">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="44a39-119">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="44a39-119">publishedFeedback</span></span>|[<span data-ttu-id="44a39-120">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="44a39-120">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="44a39-121">在向学生发布评分时所进行的反馈属性的副本。</span><span class="sxs-lookup"><span data-stu-id="44a39-121">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="44a39-122">关系</span><span class="sxs-lookup"><span data-stu-id="44a39-122">Relationships</span></span>

<span data-ttu-id="44a39-123">无</span><span class="sxs-lookup"><span data-stu-id="44a39-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44a39-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="44a39-124">JSON representation</span></span>

<span data-ttu-id="44a39-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="44a39-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "",
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