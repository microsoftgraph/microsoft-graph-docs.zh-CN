---
title: educationOutcome 资源类型
description: 对工作分配进行评分的结果
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a0a49b9a383f1e787fd2698c6d2011e11b3abedb
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173361"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="3fa9d-103">educationOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="3fa9d-103">educationOutcome resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3fa9d-104">对工作分配进行评分的结果。</span><span class="sxs-lookup"><span data-stu-id="3fa9d-104">The result of grading an assignment.</span></span> <span data-ttu-id="3fa9d-105">这是一个基本类;派生的类型为[educationFeedbackOutcome](educationfeedbackoutcome.md)、 [educationPointsOutcome](educationpointsoutcome.md)和[educationRubricOutcome](educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="3fa9d-105">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3fa9d-106">方法</span><span class="sxs-lookup"><span data-stu-id="3fa9d-106">Methods</span></span>

| <span data-ttu-id="3fa9d-107">方法</span><span class="sxs-lookup"><span data-stu-id="3fa9d-107">Method</span></span>       | <span data-ttu-id="3fa9d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="3fa9d-108">Return Type</span></span> | <span data-ttu-id="3fa9d-109">说明</span><span class="sxs-lookup"><span data-stu-id="3fa9d-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="3fa9d-110">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="3fa9d-110">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="3fa9d-111">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="3fa9d-111">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="3fa9d-112">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="3fa9d-112">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3fa9d-113">关系</span><span class="sxs-lookup"><span data-stu-id="3fa9d-113">Relationships</span></span>

<span data-ttu-id="3fa9d-114">无</span><span class="sxs-lookup"><span data-stu-id="3fa9d-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fa9d-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3fa9d-115">JSON representation</span></span>

<span data-ttu-id="3fa9d-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3fa9d-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOutcome",
  "baseType": "",
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