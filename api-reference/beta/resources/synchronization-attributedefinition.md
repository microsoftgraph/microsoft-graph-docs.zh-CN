---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ac3f6e18c4775f45f6a36814ea09b16914e139d3
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218448"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="4b20d-103">attributeDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b20d-103">attributeDefinition resource type</span></span>

<span data-ttu-id="4b20d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b20d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b20d-105">描述对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4b20d-105">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="4b20d-106">属性</span><span class="sxs-lookup"><span data-stu-id="4b20d-106">Properties</span></span>

| <span data-ttu-id="4b20d-107">属性</span><span class="sxs-lookup"><span data-stu-id="4b20d-107">Property</span></span>      | <span data-ttu-id="4b20d-108">类型</span><span class="sxs-lookup"><span data-stu-id="4b20d-108">Type</span></span>      | <span data-ttu-id="4b20d-109">说明</span><span class="sxs-lookup"><span data-stu-id="4b20d-109">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="4b20d-110">式</span><span class="sxs-lookup"><span data-stu-id="4b20d-110">anchor</span></span>         |<span data-ttu-id="4b20d-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b20d-111">Boolean</span></span>    | <span data-ttu-id="4b20d-112">`true`如果该属性应用作对象的定位标记。</span><span class="sxs-lookup"><span data-stu-id="4b20d-112">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="4b20d-113">定位属性必须具有标识对象的唯一值，并且必须是不可变的。</span><span class="sxs-lookup"><span data-stu-id="4b20d-113">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="4b20d-114">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4b20d-114">Default is `false`.</span></span> <span data-ttu-id="4b20d-115">必须将对象的一个属性（且只有一个）指定为支持同步的定位点。</span><span class="sxs-lookup"><span data-stu-id="4b20d-115">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="4b20d-116">caseExact</span><span class="sxs-lookup"><span data-stu-id="4b20d-116">caseExact</span></span>      |<span data-ttu-id="4b20d-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b20d-117">Boolean</span></span>    |<span data-ttu-id="4b20d-118">`true`如果应将此属性的值视为区分大小写。</span><span class="sxs-lookup"><span data-stu-id="4b20d-118">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="4b20d-119">此设置影响同步引擎检测属性更改的方式。</span><span class="sxs-lookup"><span data-stu-id="4b20d-119">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="4b20d-120">metadata</span><span class="sxs-lookup"><span data-stu-id="4b20d-120">metadata</span></span>       |<span data-ttu-id="4b20d-121">[metadataEntry](../resources/synchronization-metadataentry.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b20d-121">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span>   |<span data-ttu-id="4b20d-122">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="4b20d-122">Additional extension properties.</span></span> <span data-ttu-id="4b20d-123">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="4b20d-123">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="4b20d-124">多</span><span class="sxs-lookup"><span data-stu-id="4b20d-124">multivalued</span></span>    |<span data-ttu-id="4b20d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b20d-125">Boolean</span></span>    |<span data-ttu-id="4b20d-126">`true`如果属性可以有多个值。</span><span class="sxs-lookup"><span data-stu-id="4b20d-126">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="4b20d-127">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="4b20d-127">Default is `false`.</span></span>|
|<span data-ttu-id="4b20d-128">mutability</span><span class="sxs-lookup"><span data-stu-id="4b20d-128">mutability</span></span>     |<span data-ttu-id="4b20d-129">字符串</span><span class="sxs-lookup"><span data-stu-id="4b20d-129">String</span></span>     |<span data-ttu-id="4b20d-130">属性的 mutability。</span><span class="sxs-lookup"><span data-stu-id="4b20d-130">An attribute's mutability.</span></span> <span data-ttu-id="4b20d-131">可能的值为`ReadWrite`： `ReadOnly`、 `Immutable`、 `WriteOnly`、。</span><span class="sxs-lookup"><span data-stu-id="4b20d-131">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="4b20d-132">默认值为 `ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="4b20d-132">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="4b20d-133">name</span><span class="sxs-lookup"><span data-stu-id="4b20d-133">name</span></span>           |<span data-ttu-id="4b20d-134">String</span><span class="sxs-lookup"><span data-stu-id="4b20d-134">String</span></span>     |<span data-ttu-id="4b20d-135">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="4b20d-135">Name of the attribute.</span></span> <span data-ttu-id="4b20d-136">在对象定义中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="4b20d-136">Must be unique within the object definition.</span></span> <span data-ttu-id="4b20d-137">不可为空。</span><span class="sxs-lookup"><span data-stu-id="4b20d-137">Not nullable.</span></span>|
|<span data-ttu-id="4b20d-138">必需</span><span class="sxs-lookup"><span data-stu-id="4b20d-138">required</span></span>       |<span data-ttu-id="4b20d-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="4b20d-139">Boolean</span></span>    |<span data-ttu-id="4b20d-140">`true`if 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="4b20d-140">`true` if attribute is required.</span></span> <span data-ttu-id="4b20d-141">如果缺少任何必需的属性，则不能创建对象。</span><span class="sxs-lookup"><span data-stu-id="4b20d-141">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="4b20d-142">如果在同步过程中，所需的属性没有任何值，则将使用默认值。</span><span class="sxs-lookup"><span data-stu-id="4b20d-142">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="4b20d-143">如果默认值未设置，则同步将记录一个错误。</span><span class="sxs-lookup"><span data-stu-id="4b20d-143">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="4b20d-144">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="4b20d-144">referencedObjects</span></span>|<span data-ttu-id="4b20d-145">[referencedObject](../resources/synchronization-referencedobject.md)集合</span><span class="sxs-lookup"><span data-stu-id="4b20d-145">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="4b20d-146">对于 " `reference`类型" 的属性，列出引用的对象（例如`manager` ，属性将`User`作为被引用对象的列表）。</span><span class="sxs-lookup"><span data-stu-id="4b20d-146">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="4b20d-147">type</span><span class="sxs-lookup"><span data-stu-id="4b20d-147">type</span></span>           |<span data-ttu-id="4b20d-148">字符串</span><span class="sxs-lookup"><span data-stu-id="4b20d-148">String</span></span>     |<span data-ttu-id="4b20d-149">属性值类型。</span><span class="sxs-lookup"><span data-stu-id="4b20d-149">Attribute value type.</span></span> <span data-ttu-id="4b20d-150">可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。</span><span class="sxs-lookup"><span data-stu-id="4b20d-150">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="4b20d-151">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="4b20d-151">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b20d-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b20d-152">JSON representation</span></span>

<span data-ttu-id="4b20d-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b20d-153">The following is a JSON representation of the resource.</span></span>

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
