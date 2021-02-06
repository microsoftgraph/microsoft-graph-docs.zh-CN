---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 34503f3edf15542db449d56e5211cd33b3d9132e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128811"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="1a98a-103">attributeDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a98a-103">attributeDefinition resource type</span></span>

<span data-ttu-id="1a98a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a98a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a98a-105">描述对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1a98a-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="1a98a-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a98a-106">Properties</span></span>

| <span data-ttu-id="1a98a-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a98a-107">Property</span></span>      | <span data-ttu-id="1a98a-108">类型</span><span class="sxs-lookup"><span data-stu-id="1a98a-108">Type</span></span>      | <span data-ttu-id="1a98a-109">说明</span><span class="sxs-lookup"><span data-stu-id="1a98a-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="1a98a-110">anchor</span><span class="sxs-lookup"><span data-stu-id="1a98a-110">anchor</span></span>         |<span data-ttu-id="1a98a-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a98a-111">Boolean</span></span>    | <span data-ttu-id="1a98a-112">`true` 属性是否用作对象的定位标记。</span><span class="sxs-lookup"><span data-stu-id="1a98a-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="1a98a-113">定位属性必须具有标识对象的唯一值，并且必须是不可变的。</span><span class="sxs-lookup"><span data-stu-id="1a98a-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="1a98a-114">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="1a98a-114">Default is `false`.</span></span> <span data-ttu-id="1a98a-115">必须将一个（且只有一个）对象的属性指定为支持同步的定位标记。</span><span class="sxs-lookup"><span data-stu-id="1a98a-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="1a98a-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="1a98a-116">caseExact</span></span>      |<span data-ttu-id="1a98a-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a98a-117">Boolean</span></span>    |<span data-ttu-id="1a98a-118">`true` 如果应当将此属性的值视为区分大小写。</span><span class="sxs-lookup"><span data-stu-id="1a98a-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="1a98a-119">此设置会影响同步引擎检测属性的更改。</span><span class="sxs-lookup"><span data-stu-id="1a98a-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="1a98a-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="1a98a-120">flowNullValues</span></span> |<span data-ttu-id="1a98a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a98a-121">Boolean</span></span>    |<span data-ttu-id="1a98a-122">如果为"true"，则属性为 null 值。</span><span class="sxs-lookup"><span data-stu-id="1a98a-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="1a98a-123">metadata</span><span class="sxs-lookup"><span data-stu-id="1a98a-123">metadata</span></span>       |<span data-ttu-id="1a98a-124">[metadataEntry](../resources/synchronization-metadataentry.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a98a-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="1a98a-125">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="1a98a-125">Additional extension properties.</span></span> <span data-ttu-id="1a98a-126">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="1a98a-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="1a98a-127">multivalued</span><span class="sxs-lookup"><span data-stu-id="1a98a-127">multivalued</span></span>    |<span data-ttu-id="1a98a-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a98a-128">Boolean</span></span>    |<span data-ttu-id="1a98a-129">`true` 如果一个属性可以有多个值。</span><span class="sxs-lookup"><span data-stu-id="1a98a-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="1a98a-130">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="1a98a-130">Default is `false`.</span></span>|
|<span data-ttu-id="1a98a-131">可变性</span><span class="sxs-lookup"><span data-stu-id="1a98a-131">mutability</span></span>     |<span data-ttu-id="1a98a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="1a98a-132">String</span></span>     |<span data-ttu-id="1a98a-133">属性的可变性。</span><span class="sxs-lookup"><span data-stu-id="1a98a-133">An attribute's mutability.</span></span> <span data-ttu-id="1a98a-134">可能的值是：  `ReadWrite` `ReadOnly` ， ， `Immutable` `WriteOnly` 。</span><span class="sxs-lookup"><span data-stu-id="1a98a-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="1a98a-135">默认值为 `ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="1a98a-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="1a98a-136">name</span><span class="sxs-lookup"><span data-stu-id="1a98a-136">name</span></span>           |<span data-ttu-id="1a98a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="1a98a-137">String</span></span>     |<span data-ttu-id="1a98a-138">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="1a98a-138">Name of the attribute.</span></span> <span data-ttu-id="1a98a-139">在对象定义中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="1a98a-139">Must be unique within the object definition.</span></span> <span data-ttu-id="1a98a-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="1a98a-140">Not nullable.</span></span>|
|<span data-ttu-id="1a98a-141">必需</span><span class="sxs-lookup"><span data-stu-id="1a98a-141">required</span></span>       |<span data-ttu-id="1a98a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a98a-142">Boolean</span></span>    |<span data-ttu-id="1a98a-143">`true` 如果属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="1a98a-143">`true` if attribute is required.</span></span> <span data-ttu-id="1a98a-144">如果缺少任何必需的属性，则不能创建对象。</span><span class="sxs-lookup"><span data-stu-id="1a98a-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="1a98a-145">如果在同步期间，所需的属性没有值，则使用默认值。</span><span class="sxs-lookup"><span data-stu-id="1a98a-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="1a98a-146">如果未设置默认值，同步将记录错误。</span><span class="sxs-lookup"><span data-stu-id="1a98a-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="1a98a-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="1a98a-147">referencedObjects</span></span>|<span data-ttu-id="1a98a-148">[referencedObject](../resources/synchronization-referencedobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1a98a-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="1a98a-149">对于具有类型的属性，列出引用的对象 (例如，该属性将作为引用的对象列表 `reference` `manager` `User`) 。</span><span class="sxs-lookup"><span data-stu-id="1a98a-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="1a98a-150">type</span><span class="sxs-lookup"><span data-stu-id="1a98a-150">type</span></span>           |<span data-ttu-id="1a98a-151">字符串</span><span class="sxs-lookup"><span data-stu-id="1a98a-151">String</span></span>     |<span data-ttu-id="1a98a-152">属性值类型。</span><span class="sxs-lookup"><span data-stu-id="1a98a-152">Attribute value type.</span></span> <span data-ttu-id="1a98a-153">可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。</span><span class="sxs-lookup"><span data-stu-id="1a98a-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="1a98a-154">默认值为“`String`”。</span><span class="sxs-lookup"><span data-stu-id="1a98a-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a98a-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a98a-155">JSON representation</span></span>

<span data-ttu-id="1a98a-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a98a-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attributeDefinition"
}-->

```json
{
  "anchor": true,
  "caseExact": true,
  "defaultValue": "String",
  "flowNullValues": true,
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "multivalued": true,
  "mutability": "String",
  "name": "String",
  "referencedObjects": [{"@odata.type": "microsoft.graph.referencedObject"}],
  "required": true,
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


