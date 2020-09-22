---
title: educationFeedbackOutcome 资源类型
description: 以文本形式提供反馈的 educationOutcome。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b1b768fbb87804d2df16e6300cc14d71283461c0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095462"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="f3c96-103">educationFeedbackOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3c96-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="f3c96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3c96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f3c96-105">以文本形式表示对 [educationOutcome](educationoutcome.md) 对象的反馈。</span><span class="sxs-lookup"><span data-stu-id="f3c96-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="f3c96-106">方法</span><span class="sxs-lookup"><span data-stu-id="f3c96-106">Methods</span></span>

| <span data-ttu-id="f3c96-107">方法</span><span class="sxs-lookup"><span data-stu-id="f3c96-107">Method</span></span>       | <span data-ttu-id="f3c96-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f3c96-108">Return Type</span></span> | <span data-ttu-id="f3c96-109">说明</span><span class="sxs-lookup"><span data-stu-id="f3c96-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f3c96-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="f3c96-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="f3c96-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="f3c96-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="f3c96-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="f3c96-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f3c96-113">属性</span><span class="sxs-lookup"><span data-stu-id="f3c96-113">Properties</span></span>

| <span data-ttu-id="f3c96-114">属性</span><span class="sxs-lookup"><span data-stu-id="f3c96-114">Property</span></span>     | <span data-ttu-id="f3c96-115">类型</span><span class="sxs-lookup"><span data-stu-id="f3c96-115">Type</span></span>        | <span data-ttu-id="f3c96-116">说明</span><span class="sxs-lookup"><span data-stu-id="f3c96-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f3c96-117">反馈</span><span class="sxs-lookup"><span data-stu-id="f3c96-117">feedback</span></span>|[<span data-ttu-id="f3c96-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="f3c96-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="f3c96-119">教师对学生的书面反馈。</span><span class="sxs-lookup"><span data-stu-id="f3c96-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="f3c96-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="f3c96-120">publishedFeedback</span></span>|[<span data-ttu-id="f3c96-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="f3c96-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="f3c96-122">在向学生发布评分时所进行的反馈属性的副本。</span><span class="sxs-lookup"><span data-stu-id="f3c96-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3c96-123">关系</span><span class="sxs-lookup"><span data-stu-id="f3c96-123">Relationships</span></span>

<span data-ttu-id="f3c96-124">无</span><span class="sxs-lookup"><span data-stu-id="f3c96-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3c96-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3c96-125">JSON representation</span></span>

<span data-ttu-id="f3c96-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3c96-126">The following is a JSON representation of the resource.</span></span>

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

