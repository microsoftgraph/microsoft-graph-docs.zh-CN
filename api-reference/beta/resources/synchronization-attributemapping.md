---
title: attributeMapping 资源类型
description: 定义同步过程中流给定的目标属性的值应如何。
localization_priority: Normal
ms.openlocfilehash: 16235cce73a17b462f6f44aedf0c8759277983c1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509320"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="0db27-103">attributeMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="0db27-103">attributeMapping resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0db27-104">定义同步过程中流给定的目标属性的值应如何。</span><span class="sxs-lookup"><span data-stu-id="0db27-104">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="0db27-105">属性</span><span class="sxs-lookup"><span data-stu-id="0db27-105">Properties</span></span>

| <span data-ttu-id="0db27-106">属性</span><span class="sxs-lookup"><span data-stu-id="0db27-106">Property</span></span>                  | <span data-ttu-id="0db27-107">类型</span><span class="sxs-lookup"><span data-stu-id="0db27-107">Type</span></span>                      | <span data-ttu-id="0db27-108">说明</span><span class="sxs-lookup"><span data-stu-id="0db27-108">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="0db27-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="0db27-109">defaultValue</span></span>               | <span data-ttu-id="0db27-110">字符串</span><span class="sxs-lookup"><span data-stu-id="0db27-110">String</span></span>                    |<span data-ttu-id="0db27-111">默认值用于以防**source**属性计算结果为`null`。</span><span class="sxs-lookup"><span data-stu-id="0db27-111">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="0db27-112">可选。</span><span class="sxs-lookup"><span data-stu-id="0db27-112">Optional.</span></span>|
|<span data-ttu-id="0db27-113">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="0db27-113">exportMissingReferences</span></span>    |<span data-ttu-id="0db27-114">String</span><span class="sxs-lookup"><span data-stu-id="0db27-114">String</span></span>                     |<span data-ttu-id="0db27-115">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="0db27-115">For internal use only.</span></span>|
|<span data-ttu-id="0db27-116">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="0db27-116">flowBehavior</span></span>               |<span data-ttu-id="0db27-117">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="0db27-117">attributeFlowBehavior</span></span>      |<span data-ttu-id="0db27-118">定义此属性时应可导出到目标目录。</span><span class="sxs-lookup"><span data-stu-id="0db27-118">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="0db27-119">可能的值为：`FlowWhenChanged`和`FlowAlways`。</span><span class="sxs-lookup"><span data-stu-id="0db27-119">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="0db27-120">默认值为 `FlowWhenChanged`。</span><span class="sxs-lookup"><span data-stu-id="0db27-120">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="0db27-121">flowType</span><span class="sxs-lookup"><span data-stu-id="0db27-121">flowType</span></span>                   |<span data-ttu-id="0db27-122">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="0db27-122">attributeFlowType</span></span>          |<span data-ttu-id="0db27-123">定义此属性时应更新目标目录中。</span><span class="sxs-lookup"><span data-stu-id="0db27-123">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="0db27-124">可能的值为： `Always` （默认）， `ObjectAddOnly` （仅当创建新对象）， `MultiValueAddOnly` （仅当更改正在添加新值到多值属性）。</span><span class="sxs-lookup"><span data-stu-id="0db27-124">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="0db27-125">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="0db27-125">matchingPriority</span></span>           |<span data-ttu-id="0db27-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0db27-126">Int32</span></span>                      |<span data-ttu-id="0db27-127">如果大于 0，则此属性将用于执行源和目标目录之间的对象的初始匹配。</span><span class="sxs-lookup"><span data-stu-id="0db27-127">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="0db27-128">同步引擎将尝试查找匹配对象属性使用的第一次匹配优先级最低值。</span><span class="sxs-lookup"><span data-stu-id="0db27-128">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="0db27-129">如果找不到下, 一匹配 priority 属性将使用，依此类推直到找到匹配项，或没有匹配属性会保留。</span><span class="sxs-lookup"><span data-stu-id="0db27-129">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="0db27-130">仅对于预计具有唯一的值，如电子邮件、 属性应用作匹配的属性。</span><span class="sxs-lookup"><span data-stu-id="0db27-130">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="0db27-131">源</span><span class="sxs-lookup"><span data-stu-id="0db27-131">source</span></span>                     |[<span data-ttu-id="0db27-132">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="0db27-132">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="0db27-133">定义如何值应为源对象中提取 （或转换）。</span><span class="sxs-lookup"><span data-stu-id="0db27-133">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="0db27-134">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="0db27-134">targetAttributeName</span></span>        |<span data-ttu-id="0db27-135">String</span><span class="sxs-lookup"><span data-stu-id="0db27-135">String</span></span>                     |<span data-ttu-id="0db27-136">对目标对象的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="0db27-136">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0db27-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0db27-137">JSON representation</span></span>

<span data-ttu-id="0db27-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0db27-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeMapping"
}-->

```json
{
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {"@odata.type": "microsoft.graph.attributeMappingSource"},
  "targetAttributeName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeMapping resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributemapping.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
