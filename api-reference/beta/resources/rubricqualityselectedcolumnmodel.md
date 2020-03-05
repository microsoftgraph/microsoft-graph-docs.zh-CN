---
title: rubricQualitySelectedColumnModel 资源类型
description: 指示在对 educationRubric 进行评分时教师选择的 rubricLevel
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9c8b6264a0373fb5b388cd95771d9360b867feb9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520989"
---
# <a name="rubricqualityselectedcolumnmodel-resource-type"></a><span data-ttu-id="954ce-103">rubricQualitySelectedColumnModel 资源类型</span><span class="sxs-lookup"><span data-stu-id="954ce-103">rubricQualitySelectedColumnModel resource type</span></span>

<span data-ttu-id="954ce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="954ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="954ce-105">指示在向[educationRubric](educationrubric.md)评分时教师选择的[rubricLevel](rubriclevel.md) 。</span><span class="sxs-lookup"><span data-stu-id="954ce-105">Indicates the [rubricLevel](rubriclevel.md) selected by the teacher when grading an [educationRubric](educationrubric.md).</span></span>

## <a name="properties"></a><span data-ttu-id="954ce-106">属性</span><span class="sxs-lookup"><span data-stu-id="954ce-106">Properties</span></span>

| <span data-ttu-id="954ce-107">属性</span><span class="sxs-lookup"><span data-stu-id="954ce-107">Property</span></span>     | <span data-ttu-id="954ce-108">类型</span><span class="sxs-lookup"><span data-stu-id="954ce-108">Type</span></span>        | <span data-ttu-id="954ce-109">说明</span><span class="sxs-lookup"><span data-stu-id="954ce-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="954ce-110">columnId</span><span class="sxs-lookup"><span data-stu-id="954ce-110">columnId</span></span>|<span data-ttu-id="954ce-111">String</span><span class="sxs-lookup"><span data-stu-id="954ce-111">String</span></span>|<span data-ttu-id="954ce-112">此质量所对应的所选级别的 ID。</span><span class="sxs-lookup"><span data-stu-id="954ce-112">ID of the selected level for this quality.</span></span>|
|<span data-ttu-id="954ce-113">qualityId</span><span class="sxs-lookup"><span data-stu-id="954ce-113">qualityId</span></span>|<span data-ttu-id="954ce-114">String</span><span class="sxs-lookup"><span data-stu-id="954ce-114">String</span></span>|<span data-ttu-id="954ce-115">关联质量的 ID。</span><span class="sxs-lookup"><span data-stu-id="954ce-115">ID of the associated quality.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="954ce-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="954ce-116">JSON representation</span></span>

<span data-ttu-id="954ce-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="954ce-117">The following is a JSON representation of the resource.</span></span>

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