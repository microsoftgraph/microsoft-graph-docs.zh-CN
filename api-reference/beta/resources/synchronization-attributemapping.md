---
title: attributeMapping 资源类型
description: 定义给定目标属性的值在同步期间应该如何流动。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: b5f120075b082e50a0f94f05907b413a4c4c4ec6
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128748"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="f15d6-103">attributeMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="f15d6-103">attributeMapping resource type</span></span>

<span data-ttu-id="f15d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f15d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f15d6-105">定义给定目标属性的值在同步期间应该如何流动。</span><span class="sxs-lookup"><span data-stu-id="f15d6-105">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="f15d6-106">属性</span><span class="sxs-lookup"><span data-stu-id="f15d6-106">Properties</span></span>

| <span data-ttu-id="f15d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="f15d6-107">Property</span></span>                  | <span data-ttu-id="f15d6-108">类型</span><span class="sxs-lookup"><span data-stu-id="f15d6-108">Type</span></span>                      | <span data-ttu-id="f15d6-109">说明</span><span class="sxs-lookup"><span data-stu-id="f15d6-109">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="f15d6-110">defaultValue</span><span class="sxs-lookup"><span data-stu-id="f15d6-110">defaultValue</span></span>               | <span data-ttu-id="f15d6-111">字符串</span><span class="sxs-lookup"><span data-stu-id="f15d6-111">String</span></span>                    |<span data-ttu-id="f15d6-112">在将源属性求值 **到的情况下使用的** 默认值 `null` 。</span><span class="sxs-lookup"><span data-stu-id="f15d6-112">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="f15d6-113">可选。</span><span class="sxs-lookup"><span data-stu-id="f15d6-113">Optional.</span></span>|
|<span data-ttu-id="f15d6-114">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="f15d6-114">exportMissingReferences</span></span>    |<span data-ttu-id="f15d6-115">String</span><span class="sxs-lookup"><span data-stu-id="f15d6-115">String</span></span>                     |<span data-ttu-id="f15d6-116">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="f15d6-116">For internal use only.</span></span>|
|<span data-ttu-id="f15d6-117">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="f15d6-117">flowBehavior</span></span>               |<span data-ttu-id="f15d6-118">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="f15d6-118">attributeFlowBehavior</span></span>      |<span data-ttu-id="f15d6-119">定义应何时将此属性导出到目标目录。</span><span class="sxs-lookup"><span data-stu-id="f15d6-119">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="f15d6-120">可能的值是： `FlowWhenChanged` 和 `FlowAlways` 。</span><span class="sxs-lookup"><span data-stu-id="f15d6-120">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="f15d6-121">默认值为 `FlowWhenChanged`。</span><span class="sxs-lookup"><span data-stu-id="f15d6-121">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="f15d6-122">flowType</span><span class="sxs-lookup"><span data-stu-id="f15d6-122">flowType</span></span>                   |<span data-ttu-id="f15d6-123">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="f15d6-123">attributeFlowType</span></span>          |<span data-ttu-id="f15d6-124">定义应在目标目录中更新此属性的时间。</span><span class="sxs-lookup"><span data-stu-id="f15d6-124">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="f15d6-125">可能的值是： (默认值) ， (仅在) 创建新对象时， (仅在更改向多值属性中添加新值时 `Always` `ObjectAddOnly` `MultiValueAddOnly`) 。</span><span class="sxs-lookup"><span data-stu-id="f15d6-125">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="f15d6-126">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="f15d6-126">matchingPriority</span></span>           |<span data-ttu-id="f15d6-127">Int32</span><span class="sxs-lookup"><span data-stu-id="f15d6-127">Int32</span></span>                      |<span data-ttu-id="f15d6-128">如果大于 0，则此属性将用于在源目录和目标目录之间执行对象的初始匹配。</span><span class="sxs-lookup"><span data-stu-id="f15d6-128">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="f15d6-129">同步引擎将首先尝试使用具有最低匹配优先级的属性查找匹配对象。</span><span class="sxs-lookup"><span data-stu-id="f15d6-129">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="f15d6-130">如果未找到，则使用具有下一个匹配优先级的属性，等等，直到找到匹配项或没有更多匹配的属性。</span><span class="sxs-lookup"><span data-stu-id="f15d6-130">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="f15d6-131">只有预期具有唯一值的属性（如电子邮件）才应用作匹配属性。</span><span class="sxs-lookup"><span data-stu-id="f15d6-131">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="f15d6-132">source</span><span class="sxs-lookup"><span data-stu-id="f15d6-132">source</span></span>                     |[<span data-ttu-id="f15d6-133">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="f15d6-133">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="f15d6-134">定义如何从源对象中提取 (或) 转换值。</span><span class="sxs-lookup"><span data-stu-id="f15d6-134">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="f15d6-135">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="f15d6-135">targetAttributeName</span></span>        |<span data-ttu-id="f15d6-136">字符串</span><span class="sxs-lookup"><span data-stu-id="f15d6-136">String</span></span>                     |<span data-ttu-id="f15d6-137">目标对象上属性的名称。</span><span class="sxs-lookup"><span data-stu-id="f15d6-137">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f15d6-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f15d6-138">JSON representation</span></span>

<span data-ttu-id="f15d6-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f15d6-139">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


