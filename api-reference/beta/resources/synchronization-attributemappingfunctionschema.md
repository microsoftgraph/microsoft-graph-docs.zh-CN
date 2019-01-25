---
title: attributeMappingFunctionSchema 资源类型
description: 介绍可用于中的属性映射同步过程中转换值的函数。
localization_priority: Normal
ms.openlocfilehash: e2c0139f7c797c3f519cc638561b09f611018b28
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511980"
---
# <a name="attributemappingfunctionschema-resource-type"></a><span data-ttu-id="ca050-103">attributeMappingFunctionSchema 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca050-103">attributeMappingFunctionSchema resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ca050-104">介绍可在[属性映射](synchronization-attributemapping.md)用于同步过程中转换值的函数。</span><span class="sxs-lookup"><span data-stu-id="ca050-104">Describes a function that can be used in an [attribute mapping](synchronization-attributemapping.md) to transform values during synchronization.</span></span>

## <a name="methods"></a><span data-ttu-id="ca050-105">方法</span><span class="sxs-lookup"><span data-stu-id="ca050-105">Methods</span></span>

| <span data-ttu-id="ca050-106">方法</span><span class="sxs-lookup"><span data-stu-id="ca050-106">Method</span></span>           | <span data-ttu-id="ca050-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="ca050-107">Return Type</span></span>    |<span data-ttu-id="ca050-108">说明</span><span class="sxs-lookup"><span data-stu-id="ca050-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ca050-109">List</span><span class="sxs-lookup"><span data-stu-id="ca050-109">List</span></span>](../api/synchronization-synchronizationschema-functions.md) | <span data-ttu-id="ca050-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca050-110">[attributeMappingFunctionSchema](../resources/synchronization-attributemappingfunctionschema.md) collection</span></span>|<span data-ttu-id="ca050-111">支持列表属性的映射功能。</span><span class="sxs-lookup"><span data-stu-id="ca050-111">List supported attribute mapping functions.</span></span>|

## <a name="properties"></a><span data-ttu-id="ca050-112">属性</span><span class="sxs-lookup"><span data-stu-id="ca050-112">Properties</span></span>

| <span data-ttu-id="ca050-113">属性</span><span class="sxs-lookup"><span data-stu-id="ca050-113">Property</span></span>                   | <span data-ttu-id="ca050-114">类型</span><span class="sxs-lookup"><span data-stu-id="ca050-114">Type</span></span>                      | <span data-ttu-id="ca050-115">说明</span><span class="sxs-lookup"><span data-stu-id="ca050-115">Description</span></span>    |
|:---------------------------|:-------------------------|:---------------|
|<span data-ttu-id="ca050-116">name</span><span class="sxs-lookup"><span data-stu-id="ca050-116">name</span></span>                        |<span data-ttu-id="ca050-117">String</span><span class="sxs-lookup"><span data-stu-id="ca050-117">String</span></span>                    |<span data-ttu-id="ca050-118">运算符名称。</span><span class="sxs-lookup"><span data-stu-id="ca050-118">Operator name.</span></span> |
|<span data-ttu-id="ca050-119">参数</span><span class="sxs-lookup"><span data-stu-id="ca050-119">parameters</span></span>                  |<span data-ttu-id="ca050-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md)集合</span><span class="sxs-lookup"><span data-stu-id="ca050-120">[attributeMappingParameterSchema](../resources/synchronization-attributemappingparameterschema.md) collection</span></span>  |<span data-ttu-id="ca050-121">函数参数的集合。</span><span class="sxs-lookup"><span data-stu-id="ca050-121">Collection of function parameters.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca050-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca050-122">JSON representation</span></span>

<span data-ttu-id="ca050-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca050-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMappingFunctionSchema"
}-->

```json
{
  "name": "String (identifier)",
  "parameters": [{"@odata.type": "microsoft.graph.attributeMappingParameterSchema"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMappingFunctionSchema resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemappingfunctionschema.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
