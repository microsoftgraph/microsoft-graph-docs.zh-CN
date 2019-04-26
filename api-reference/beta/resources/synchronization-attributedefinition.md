---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
ms.openlocfilehash: f9268bf61fec397c53744c9999635ba159b047f4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32582071"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="39192-103">attributeDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="39192-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39192-104">描述对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39192-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="39192-105">属性</span><span class="sxs-lookup"><span data-stu-id="39192-105">Properties</span></span>

| <span data-ttu-id="39192-106">属性</span><span class="sxs-lookup"><span data-stu-id="39192-106">Property</span></span>      | <span data-ttu-id="39192-107">类型</span><span class="sxs-lookup"><span data-stu-id="39192-107">Type</span></span>      | <span data-ttu-id="39192-108">说明</span><span class="sxs-lookup"><span data-stu-id="39192-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="39192-109">式</span><span class="sxs-lookup"><span data-stu-id="39192-109">anchor</span></span>         |<span data-ttu-id="39192-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="39192-110">Boolean</span></span>    | <span data-ttu-id="39192-111">`true`如果该属性应用作对象的定位标记。</span><span class="sxs-lookup"><span data-stu-id="39192-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="39192-112">定位属性必须具有标识对象的唯一值, 并且必须是不可变的。</span><span class="sxs-lookup"><span data-stu-id="39192-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="39192-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="39192-113">Default is `false`.</span></span> <span data-ttu-id="39192-114">必须将对象的一个属性 (且只有一个) 指定为支持同步的定位点。</span><span class="sxs-lookup"><span data-stu-id="39192-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="39192-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="39192-115">caseExact</span></span>      |<span data-ttu-id="39192-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="39192-116">Boolean</span></span>    |<span data-ttu-id="39192-117">`true`如果应将此属性的值视为区分大小写。</span><span class="sxs-lookup"><span data-stu-id="39192-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="39192-118">此设置影响同步引擎检测属性更改的方式。</span><span class="sxs-lookup"><span data-stu-id="39192-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="39192-119">metadata</span><span class="sxs-lookup"><span data-stu-id="39192-119">metadata</span></span>       |[<span data-ttu-id="39192-120">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="39192-120">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="39192-121">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="39192-121">Additional extension properties.</span></span> <span data-ttu-id="39192-122">除非明确提到, 否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="39192-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="39192-123">多</span><span class="sxs-lookup"><span data-stu-id="39192-123">multivalued</span></span>    |<span data-ttu-id="39192-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="39192-124">Boolean</span></span>    |<span data-ttu-id="39192-125">`true`如果属性可以有多个值。</span><span class="sxs-lookup"><span data-stu-id="39192-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="39192-126">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="39192-126">Default is `false`.</span></span>|
|<span data-ttu-id="39192-127">mutability</span><span class="sxs-lookup"><span data-stu-id="39192-127">mutability</span></span>     |<span data-ttu-id="39192-128">String</span><span class="sxs-lookup"><span data-stu-id="39192-128">String</span></span>     |<span data-ttu-id="39192-129">属性的 mutability。</span><span class="sxs-lookup"><span data-stu-id="39192-129">An attribute's mutability.</span></span> <span data-ttu-id="39192-130">可能的值为`ReadWrite`: `ReadOnly`、 `Immutable`、 `WriteOnly`、。</span><span class="sxs-lookup"><span data-stu-id="39192-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="39192-131">默认值为 `ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="39192-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="39192-132">name</span><span class="sxs-lookup"><span data-stu-id="39192-132">name</span></span>           |<span data-ttu-id="39192-133">String</span><span class="sxs-lookup"><span data-stu-id="39192-133">String</span></span>     |<span data-ttu-id="39192-134">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="39192-134">Name of the attribute.</span></span> <span data-ttu-id="39192-135">在对象定义中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="39192-135">Must be unique within the object definition.</span></span> <span data-ttu-id="39192-136">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="39192-136">Not nullable.</span></span>|
|<span data-ttu-id="39192-137">必需</span><span class="sxs-lookup"><span data-stu-id="39192-137">required</span></span>       |<span data-ttu-id="39192-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="39192-138">Boolean</span></span>    |<span data-ttu-id="39192-139">`true`if 属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="39192-139">`true` if attribute is required.</span></span> <span data-ttu-id="39192-140">如果缺少任何必需的属性, 则不能创建对象。</span><span class="sxs-lookup"><span data-stu-id="39192-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="39192-141">如果在同步过程中, 所需的属性没有任何值, 则将使用默认值。</span><span class="sxs-lookup"><span data-stu-id="39192-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="39192-142">如果默认值未设置, 则同步将记录一个错误。</span><span class="sxs-lookup"><span data-stu-id="39192-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="39192-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="39192-143">referencedObjects</span></span>|[<span data-ttu-id="39192-144">referencedObject</span><span class="sxs-lookup"><span data-stu-id="39192-144">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="39192-145">对于 " `reference`类型" 的属性, 列出引用的对象 (例如`manager` , 属性将`User`作为被引用对象的列表)。</span><span class="sxs-lookup"><span data-stu-id="39192-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="39192-146">type</span><span class="sxs-lookup"><span data-stu-id="39192-146">type</span></span>           |<span data-ttu-id="39192-147">String</span><span class="sxs-lookup"><span data-stu-id="39192-147">String</span></span>     |<span data-ttu-id="39192-148">属性值类型。</span><span class="sxs-lookup"><span data-stu-id="39192-148">Attribute value type.</span></span> <span data-ttu-id="39192-149">可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。</span><span class="sxs-lookup"><span data-stu-id="39192-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="39192-150">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="39192-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39192-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39192-151">JSON representation</span></span>

<span data-ttu-id="39192-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39192-152">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-attributedefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
