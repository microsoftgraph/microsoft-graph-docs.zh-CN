---
title: attributeMapping 资源类型
description: 定义如何在同步过程中传递给定目标属性的值。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7573773737f4ff4380a446cf62107e8ac26642ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078080"
---
# <a name="attributemapping-resource-type"></a><span data-ttu-id="9d0d8-103">attributeMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d0d8-103">attributeMapping resource type</span></span>

<span data-ttu-id="9d0d8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d0d8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d0d8-105">定义如何在同步过程中传递给定目标属性的值。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-105">Defines how values for the given target attribute should flow during synchronization.</span></span>

## <a name="properties"></a><span data-ttu-id="9d0d8-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d0d8-106">Properties</span></span>

| <span data-ttu-id="9d0d8-107">属性</span><span class="sxs-lookup"><span data-stu-id="9d0d8-107">Property</span></span>                  | <span data-ttu-id="9d0d8-108">类型</span><span class="sxs-lookup"><span data-stu-id="9d0d8-108">Type</span></span>                      | <span data-ttu-id="9d0d8-109">说明</span><span class="sxs-lookup"><span data-stu-id="9d0d8-109">Description</span></span>    |
|:--------------------------|:--------------------------|:---------------|
|<span data-ttu-id="9d0d8-110">默认</span><span class="sxs-lookup"><span data-stu-id="9d0d8-110">defaultValue</span></span>               | <span data-ttu-id="9d0d8-111">String</span><span class="sxs-lookup"><span data-stu-id="9d0d8-111">String</span></span>                    |<span data-ttu-id="9d0d8-112">要在对 **源** 属性进行求值的情况下使用的默认值 `null` 。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-112">Default value to be used in case the **source** property was evaluated to `null`.</span></span> <span data-ttu-id="9d0d8-113">可选。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-113">Optional.</span></span>|
|<span data-ttu-id="9d0d8-114">exportMissingReferences</span><span class="sxs-lookup"><span data-stu-id="9d0d8-114">exportMissingReferences</span></span>    |<span data-ttu-id="9d0d8-115">String</span><span class="sxs-lookup"><span data-stu-id="9d0d8-115">String</span></span>                     |<span data-ttu-id="9d0d8-116">仅供内部使用。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-116">For internal use only.</span></span>|
|<span data-ttu-id="9d0d8-117">flowBehavior</span><span class="sxs-lookup"><span data-stu-id="9d0d8-117">flowBehavior</span></span>               |<span data-ttu-id="9d0d8-118">attributeFlowBehavior</span><span class="sxs-lookup"><span data-stu-id="9d0d8-118">attributeFlowBehavior</span></span>      |<span data-ttu-id="9d0d8-119">定义何时应将此属性导出到目标目录。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-119">Defines when this attribute should be exported to the target directory.</span></span> <span data-ttu-id="9d0d8-120">可能的值为： `FlowWhenChanged` 和 `FlowAlways` 。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-120">Possible values are: `FlowWhenChanged` and `FlowAlways`.</span></span> <span data-ttu-id="9d0d8-121">默认值为 `FlowWhenChanged`。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-121">Default is `FlowWhenChanged`.</span></span> |
|<span data-ttu-id="9d0d8-122">flowType</span><span class="sxs-lookup"><span data-stu-id="9d0d8-122">flowType</span></span>                   |<span data-ttu-id="9d0d8-123">attributeFlowType</span><span class="sxs-lookup"><span data-stu-id="9d0d8-123">attributeFlowType</span></span>          |<span data-ttu-id="9d0d8-124">定义应何时在目标目录中更新此属性。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-124">Defines when this attribute should be updated in the target directory.</span></span> <span data-ttu-id="9d0d8-125">可能的值包括： `Always` (默认) ， `ObjectAddOnly` 仅在创建新对象时 () ， `MultiValueAddOnly` (仅当更改将新值添加到多值属性) 时。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-125">Possible values are: `Always` (default), `ObjectAddOnly` (only when new object is created), `MultiValueAddOnly` (only when the change is adding new values to a multi-valued attribute).</span></span> |
|<span data-ttu-id="9d0d8-126">matchingPriority</span><span class="sxs-lookup"><span data-stu-id="9d0d8-126">matchingPriority</span></span>           |<span data-ttu-id="9d0d8-127">Int32</span><span class="sxs-lookup"><span data-stu-id="9d0d8-127">Int32</span></span>                      |<span data-ttu-id="9d0d8-128">如果高于0，则此属性将用于执行源目录和目标目录之间的对象的初始匹配。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-128">If higher than 0, this attribute will be used to perform an initial match of the objects between source and target directories.</span></span> <span data-ttu-id="9d0d8-129">同步引擎将尝试使用具有最小匹配优先级值的属性来查找匹配的对象。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-129">The synchronization engine will try to find the matching object using attribute with lowest value of matching priority first.</span></span> <span data-ttu-id="9d0d8-130">如果未找到，则将使用具有下一个匹配的优先级的属性，在找到匹配项或不留下更多匹配属性的情况下，将使用该属性。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-130">If not found, the attribute with the next matching priority will be used, and so on a until match is found or no more matching attributes are left.</span></span> <span data-ttu-id="9d0d8-131">应仅将应具有唯一值的属性（如电子邮件）用作匹配属性。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-131">Only attributes that are expected to have unique values, such as email, should be used as matching attributes.</span></span>|
|<span data-ttu-id="9d0d8-132">source</span><span class="sxs-lookup"><span data-stu-id="9d0d8-132">source</span></span>                     |[<span data-ttu-id="9d0d8-133">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="9d0d8-133">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)     | <span data-ttu-id="9d0d8-134">定义应如何在源对象中提取 (或转换) 的值。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-134">Defines how a value should be extracted (or transformed) from the source object.</span></span> |
|<span data-ttu-id="9d0d8-135">targetAttributeName</span><span class="sxs-lookup"><span data-stu-id="9d0d8-135">targetAttributeName</span></span>        |<span data-ttu-id="9d0d8-136">String</span><span class="sxs-lookup"><span data-stu-id="9d0d8-136">String</span></span>                     |<span data-ttu-id="9d0d8-137">目标对象上的属性的名称。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-137">Name of the attribute on the target object.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d0d8-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d0d8-138">JSON representation</span></span>

<span data-ttu-id="9d0d8-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d0d8-139">The following is a JSON representation of the resource.</span></span>

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


