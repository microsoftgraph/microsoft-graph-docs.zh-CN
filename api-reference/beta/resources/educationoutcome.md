---
title: educationOutcome 资源类型
description: 对工作分配评分的结果
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 788985e5e63272fea31e579c2da4472ec065dfc5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153621"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="1daf9-103">educationOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="1daf9-103">educationOutcome resource type</span></span>

<span data-ttu-id="1daf9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1daf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1daf9-105">对工作分配进行评分的结果。</span><span class="sxs-lookup"><span data-stu-id="1daf9-105">The result of grading an assignment.</span></span> <span data-ttu-id="1daf9-106">这是一个基类;派生的类型是[educationFeedbackOutcome](educationfeedbackoutcome.md) [、educationPointsOutcome](educationpointsoutcome.md)[和 educationRubricOutcome。](educationrubricoutcome.md)</span><span class="sxs-lookup"><span data-stu-id="1daf9-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1daf9-107">方法</span><span class="sxs-lookup"><span data-stu-id="1daf9-107">Methods</span></span>

| <span data-ttu-id="1daf9-108">方法</span><span class="sxs-lookup"><span data-stu-id="1daf9-108">Method</span></span>       | <span data-ttu-id="1daf9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1daf9-109">Return Type</span></span> | <span data-ttu-id="1daf9-110">说明</span><span class="sxs-lookup"><span data-stu-id="1daf9-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1daf9-111">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="1daf9-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="1daf9-112">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="1daf9-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="1daf9-113">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="1daf9-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="1daf9-114">关系</span><span class="sxs-lookup"><span data-stu-id="1daf9-114">Relationships</span></span>

<span data-ttu-id="1daf9-115">无</span><span class="sxs-lookup"><span data-stu-id="1daf9-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1daf9-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1daf9-116">JSON representation</span></span>

<span data-ttu-id="1daf9-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1daf9-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOutcome resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

