---
title: educationFeedbackOutcome 资源类型
description: 以文本形式提供反馈的 educationOutcome。
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 3dd9dd01c19306d66ac91578a5430ff26667b0e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502128"
---
# <a name="educationfeedbackoutcome-resource-type"></a><span data-ttu-id="96acf-103">educationFeedbackOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="96acf-103">educationFeedbackOutcome resource type</span></span>

<span data-ttu-id="96acf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="96acf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96acf-105">以文本形式表示对[educationOutcome](educationoutcome.md)对象的反馈。</span><span class="sxs-lookup"><span data-stu-id="96acf-105">Represents feedback on an [educationOutcome](educationoutcome.md) object in the form of text.</span></span> 

## <a name="methods"></a><span data-ttu-id="96acf-106">方法</span><span class="sxs-lookup"><span data-stu-id="96acf-106">Methods</span></span>

| <span data-ttu-id="96acf-107">方法</span><span class="sxs-lookup"><span data-stu-id="96acf-107">Method</span></span>       | <span data-ttu-id="96acf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="96acf-108">Return Type</span></span> | <span data-ttu-id="96acf-109">说明</span><span class="sxs-lookup"><span data-stu-id="96acf-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="96acf-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="96acf-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="96acf-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="96acf-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="96acf-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="96acf-112">Update educationOutcome object.</span></span> |

## <a name="properties"></a><span data-ttu-id="96acf-113">属性</span><span class="sxs-lookup"><span data-stu-id="96acf-113">Properties</span></span>

| <span data-ttu-id="96acf-114">属性</span><span class="sxs-lookup"><span data-stu-id="96acf-114">Property</span></span>     | <span data-ttu-id="96acf-115">类型</span><span class="sxs-lookup"><span data-stu-id="96acf-115">Type</span></span>        | <span data-ttu-id="96acf-116">说明</span><span class="sxs-lookup"><span data-stu-id="96acf-116">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="96acf-117">反馈</span><span class="sxs-lookup"><span data-stu-id="96acf-117">feedback</span></span>|[<span data-ttu-id="96acf-118">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="96acf-118">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="96acf-119">教师对学生的书面反馈。</span><span class="sxs-lookup"><span data-stu-id="96acf-119">Teacher's written feedback to the student.</span></span>|
|<span data-ttu-id="96acf-120">publishedFeedback</span><span class="sxs-lookup"><span data-stu-id="96acf-120">publishedFeedback</span></span>|[<span data-ttu-id="96acf-121">educationFeedback</span><span class="sxs-lookup"><span data-stu-id="96acf-121">educationFeedback</span></span>](educationfeedback.md)|<span data-ttu-id="96acf-122">在向学生发布评分时所进行的反馈属性的副本。</span><span class="sxs-lookup"><span data-stu-id="96acf-122">A copy of the feedback property that is made when the grade is released to the student.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96acf-123">关系</span><span class="sxs-lookup"><span data-stu-id="96acf-123">Relationships</span></span>

<span data-ttu-id="96acf-124">无</span><span class="sxs-lookup"><span data-stu-id="96acf-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96acf-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96acf-125">JSON representation</span></span>

<span data-ttu-id="96acf-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96acf-126">The following is a JSON representation of the resource.</span></span>

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