---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: a9c50721c1ee19505edc2507313cc346a6adabfd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956811"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="626a7-103">attributeDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="626a7-103">attributeDefinition resource type</span></span>

<span data-ttu-id="626a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="626a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="626a7-105">描述对象的属性。</span><span class="sxs-lookup"><span data-stu-id="626a7-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="626a7-106">属性</span><span class="sxs-lookup"><span data-stu-id="626a7-106">Properties</span></span>

| <span data-ttu-id="626a7-107">属性</span><span class="sxs-lookup"><span data-stu-id="626a7-107">Property</span></span>      | <span data-ttu-id="626a7-108">类型</span><span class="sxs-lookup"><span data-stu-id="626a7-108">Type</span></span>      | <span data-ttu-id="626a7-109">说明</span><span class="sxs-lookup"><span data-stu-id="626a7-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="626a7-110">anchor</span><span class="sxs-lookup"><span data-stu-id="626a7-110">anchor</span></span>         |<span data-ttu-id="626a7-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="626a7-111">Boolean</span></span>    | <span data-ttu-id="626a7-112">`true` 属性是否用作对象的定位标记。</span><span class="sxs-lookup"><span data-stu-id="626a7-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="626a7-113">定位属性必须具有标识对象的唯一值，并且必须是不可变的。</span><span class="sxs-lookup"><span data-stu-id="626a7-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="626a7-114">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="626a7-114">Default is `false`.</span></span> <span data-ttu-id="626a7-115">必须将对象属性中的一个（且只有一个）指定为支持同步的定位标记。</span><span class="sxs-lookup"><span data-stu-id="626a7-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="626a7-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="626a7-116">caseExact</span></span>      |<span data-ttu-id="626a7-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="626a7-117">Boolean</span></span>    |<span data-ttu-id="626a7-118">`true` 如果此属性的值应视为区分大小写。</span><span class="sxs-lookup"><span data-stu-id="626a7-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="626a7-119">此设置会影响同步引擎检测属性更改。</span><span class="sxs-lookup"><span data-stu-id="626a7-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="626a7-120">flowNullValues</span><span class="sxs-lookup"><span data-stu-id="626a7-120">flowNullValues</span></span> |<span data-ttu-id="626a7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="626a7-121">Boolean</span></span>    |<span data-ttu-id="626a7-122">"true"表示允许属性为 null 值。</span><span class="sxs-lookup"><span data-stu-id="626a7-122">'true' to allow null values for attributes.</span></span>|
|<span data-ttu-id="626a7-123">metadata</span><span class="sxs-lookup"><span data-stu-id="626a7-123">metadata</span></span>       |<span data-ttu-id="626a7-124">[metadataEntry](../resources/synchronization-metadataentry.md) 集合</span><span class="sxs-lookup"><span data-stu-id="626a7-124">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="626a7-125">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="626a7-125">Additional extension properties.</span></span> <span data-ttu-id="626a7-126">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="626a7-126">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="626a7-127">多值</span><span class="sxs-lookup"><span data-stu-id="626a7-127">multivalued</span></span>    |<span data-ttu-id="626a7-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="626a7-128">Boolean</span></span>    |<span data-ttu-id="626a7-129">`true` 如果一个属性可以有多个值。</span><span class="sxs-lookup"><span data-stu-id="626a7-129">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="626a7-130">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="626a7-130">Default is `false`.</span></span>|
|<span data-ttu-id="626a7-131">可变性</span><span class="sxs-lookup"><span data-stu-id="626a7-131">mutability</span></span>     |<span data-ttu-id="626a7-132">可变性</span><span class="sxs-lookup"><span data-stu-id="626a7-132">mutability</span></span>     |<span data-ttu-id="626a7-133">属性的可变性。</span><span class="sxs-lookup"><span data-stu-id="626a7-133">An attribute's mutability.</span></span> <span data-ttu-id="626a7-134">可能的值是 `ReadWrite` `ReadOnly` `Immutable` ：、、、。 `WriteOnly`</span><span class="sxs-lookup"><span data-stu-id="626a7-134">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="626a7-135">默认值为 `ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="626a7-135">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="626a7-136">name</span><span class="sxs-lookup"><span data-stu-id="626a7-136">name</span></span>           |<span data-ttu-id="626a7-137">String</span><span class="sxs-lookup"><span data-stu-id="626a7-137">String</span></span>     |<span data-ttu-id="626a7-138">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="626a7-138">Name of the attribute.</span></span> <span data-ttu-id="626a7-139">在对象定义中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="626a7-139">Must be unique within the object definition.</span></span> <span data-ttu-id="626a7-140">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="626a7-140">Not nullable.</span></span>|
|<span data-ttu-id="626a7-141">必需</span><span class="sxs-lookup"><span data-stu-id="626a7-141">required</span></span>       |<span data-ttu-id="626a7-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="626a7-142">Boolean</span></span>    |<span data-ttu-id="626a7-143">`true` 如果 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="626a7-143">`true` if attribute is required.</span></span> <span data-ttu-id="626a7-144">如果缺少任何必需的属性，则不能创建对象。</span><span class="sxs-lookup"><span data-stu-id="626a7-144">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="626a7-145">如果在同步期间，所需的属性没有值，则使用默认值。</span><span class="sxs-lookup"><span data-stu-id="626a7-145">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="626a7-146">如果未设置默认值，则同步将记录错误。</span><span class="sxs-lookup"><span data-stu-id="626a7-146">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="626a7-147">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="626a7-147">referencedObjects</span></span>|<span data-ttu-id="626a7-148">[referencedObject](../resources/synchronization-referencedobject.md) 集合</span><span class="sxs-lookup"><span data-stu-id="626a7-148">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="626a7-149">对于类型为 的属性，列出引用 (例如，该属性将列出为引用 `reference` `manager` `User` 的对象) 。</span><span class="sxs-lookup"><span data-stu-id="626a7-149">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="626a7-150">type</span><span class="sxs-lookup"><span data-stu-id="626a7-150">type</span></span>           |<span data-ttu-id="626a7-151">attributeType</span><span class="sxs-lookup"><span data-stu-id="626a7-151">attributeType</span></span>     |<span data-ttu-id="626a7-152">属性值类型。</span><span class="sxs-lookup"><span data-stu-id="626a7-152">Attribute value type.</span></span> <span data-ttu-id="626a7-153">可能的值是 `String` `Integer` `Reference` ：、、、、、。 `Binary` `Boolean` `DateTime`</span><span class="sxs-lookup"><span data-stu-id="626a7-153">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`,`DateTime`.</span></span> <span data-ttu-id="626a7-154">默认值为“`String`”。</span><span class="sxs-lookup"><span data-stu-id="626a7-154">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="626a7-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="626a7-155">JSON representation</span></span>

<span data-ttu-id="626a7-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="626a7-156">The following is a JSON representation of the resource.</span></span>

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


