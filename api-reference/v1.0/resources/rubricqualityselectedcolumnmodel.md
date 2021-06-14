---
title: rubricQualitySelectedColumnModel 资源类型
description: 指示教师在对 educationRubric 进行评分时选择的评分标准。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9e69fa26d97684db4964ffba3d268ee1d1c11b44
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911403"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="53192-103">rubricQualitySelectedColumnModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="53192-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="53192-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53192-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="53192-105">指示教师 [在评分](rubriclevel.md) [educationRubric](educationrubric.md)时选择的评分标准。</span><span class="sxs-lookup"><span data-stu-id="53192-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="53192-106">属性</span><span class="sxs-lookup"><span data-stu-id="53192-106">Properties</span></span>

| <span data-ttu-id="53192-107">属性</span><span class="sxs-lookup"><span data-stu-id="53192-107">Property</span></span>     | <span data-ttu-id="53192-108">类型</span><span class="sxs-lookup"><span data-stu-id="53192-108">Type</span></span>        | <span data-ttu-id="53192-109">说明</span><span class="sxs-lookup"><span data-stu-id="53192-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="53192-110">columnId</span><span class="sxs-lookup"><span data-stu-id="53192-110">columnId</span></span>|<span data-ttu-id="53192-111">String</span><span class="sxs-lookup"><span data-stu-id="53192-111">String</span></span>|<span data-ttu-id="53192-112">此质量的选定级别的 ID。</span><span class="sxs-lookup"><span data-stu-id="53192-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="53192-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="53192-113">qualityId</span></span>|<span data-ttu-id="53192-114">String</span><span class="sxs-lookup"><span data-stu-id="53192-114">String</span></span>|<span data-ttu-id="53192-115">关联质量的 ID。</span><span class="sxs-lookup"><span data-stu-id="53192-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53192-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53192-116">JSON representation</span></span>

<span data-ttu-id="53192-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53192-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel",
  "baseType": null
}-->

```json
{
  "columnId": "String",
  "qualityId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "rubricQualitySelectedColumnModel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

