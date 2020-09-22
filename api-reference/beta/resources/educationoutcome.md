---
title: educationOutcome 资源类型
description: 对工作分配进行评分的结果
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 129e48b5d1101aaf9ab6ab7eb8c89a92b41a6ac7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081709"
---
# <a name="educationoutcome-resource-type"></a><span data-ttu-id="7a25b-103">educationOutcome 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a25b-103">educationOutcome resource type</span></span>

<span data-ttu-id="7a25b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a25b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a25b-105">对工作分配进行评分的结果。</span><span class="sxs-lookup"><span data-stu-id="7a25b-105">The result of grading an assignment.</span></span> <span data-ttu-id="7a25b-106">这是一个基本类;派生的类型为 [educationFeedbackOutcome](educationfeedbackoutcome.md)、 [educationPointsOutcome](educationpointsoutcome.md)和 [educationRubricOutcome](educationrubricoutcome.md)。</span><span class="sxs-lookup"><span data-stu-id="7a25b-106">This is a base class; the derived types are [educationFeedbackOutcome](educationfeedbackoutcome.md), [educationPointsOutcome](educationpointsoutcome.md), and [educationRubricOutcome](educationrubricoutcome.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7a25b-107">方法</span><span class="sxs-lookup"><span data-stu-id="7a25b-107">Methods</span></span>

| <span data-ttu-id="7a25b-108">方法</span><span class="sxs-lookup"><span data-stu-id="7a25b-108">Method</span></span>       | <span data-ttu-id="7a25b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="7a25b-109">Return Type</span></span> | <span data-ttu-id="7a25b-110">说明</span><span class="sxs-lookup"><span data-stu-id="7a25b-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7a25b-111">更新 educationOutcome</span><span class="sxs-lookup"><span data-stu-id="7a25b-111">Update educationOutcome</span></span>](../api/educationoutcome-update.md) | [<span data-ttu-id="7a25b-112">educationOutcome</span><span class="sxs-lookup"><span data-stu-id="7a25b-112">educationOutcome</span></span>](educationoutcome.md) | <span data-ttu-id="7a25b-113">更新 educationOutcome 对象。</span><span class="sxs-lookup"><span data-stu-id="7a25b-113">Update educationOutcome object.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7a25b-114">关系</span><span class="sxs-lookup"><span data-stu-id="7a25b-114">Relationships</span></span>

<span data-ttu-id="7a25b-115">无</span><span class="sxs-lookup"><span data-stu-id="7a25b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a25b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a25b-116">JSON representation</span></span>

<span data-ttu-id="7a25b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a25b-117">The following is a JSON representation of the resource.</span></span>

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

