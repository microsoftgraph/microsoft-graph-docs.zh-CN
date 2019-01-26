---
title: attributeDefinition 资源类型
description: 描述对象的属性。
localization_priority: Normal
ms.openlocfilehash: 30c9d6b2f57aaadd9ef17982b1affa765bbfbec0
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571861"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="8bfc5-103">attributeDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bfc5-103">attributeDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bfc5-104">描述对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-104">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="8bfc5-105">属性</span><span class="sxs-lookup"><span data-stu-id="8bfc5-105">Properties</span></span>

| <span data-ttu-id="8bfc5-106">属性</span><span class="sxs-lookup"><span data-stu-id="8bfc5-106">Property</span></span>      | <span data-ttu-id="8bfc5-107">类型</span><span class="sxs-lookup"><span data-stu-id="8bfc5-107">Type</span></span>      | <span data-ttu-id="8bfc5-108">说明</span><span class="sxs-lookup"><span data-stu-id="8bfc5-108">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="8bfc5-109">定位</span><span class="sxs-lookup"><span data-stu-id="8bfc5-109">anchor</span></span>         |<span data-ttu-id="8bfc5-110">布尔值</span><span class="sxs-lookup"><span data-stu-id="8bfc5-110">Boolean</span></span>    | <span data-ttu-id="8bfc5-111">`true`如果属性应用作对象的定位标记。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-111">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="8bfc5-112">定位属性必须具有识别对象的唯一值，并且必须变。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-112">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="8bfc5-113">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-113">Default is `false`.</span></span> <span data-ttu-id="8bfc5-114">有，并且只有一个对象的属性必须被指定为定位标记为支持同步。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-114">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="8bfc5-115">caseExact</span><span class="sxs-lookup"><span data-stu-id="8bfc5-115">caseExact</span></span>      |<span data-ttu-id="8bfc5-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="8bfc5-116">Boolean</span></span>    |<span data-ttu-id="8bfc5-117">`true`如果此属性的值应处理，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-117">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="8bfc5-118">此设置会影响如何同步引擎检测到的属性的更改。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-118">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="8bfc5-119">元数据</span><span class="sxs-lookup"><span data-stu-id="8bfc5-119">metadata</span></span>       |<span data-ttu-id="8bfc5-120">[metadataEntry](../resources/synchronization-metadataentry.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bfc5-120">[metadataEntry](../resources/synchronization-metadataentry.md) collection</span></span> |<span data-ttu-id="8bfc5-121">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-121">Additional extension properties.</span></span> <span data-ttu-id="8bfc5-122">除非明确提到，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-122">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="8bfc5-123">多值</span><span class="sxs-lookup"><span data-stu-id="8bfc5-123">multivalued</span></span>    |<span data-ttu-id="8bfc5-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="8bfc5-124">Boolean</span></span>    |<span data-ttu-id="8bfc5-125">`true`如果属性可以有多个值。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-125">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="8bfc5-126">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-126">Default is `false`.</span></span>|
|<span data-ttu-id="8bfc5-127">mutability</span><span class="sxs-lookup"><span data-stu-id="8bfc5-127">mutability</span></span>     |<span data-ttu-id="8bfc5-128">String</span><span class="sxs-lookup"><span data-stu-id="8bfc5-128">String</span></span>     |<span data-ttu-id="8bfc5-129">属性可变性。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-129">An attribute's mutability.</span></span> <span data-ttu-id="8bfc5-130">可能的值为： `ReadWrite`， `ReadOnly`， `Immutable`， `WriteOnly`。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-130">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="8bfc5-131">默认值为 `ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-131">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="8bfc5-132">name</span><span class="sxs-lookup"><span data-stu-id="8bfc5-132">name</span></span>           |<span data-ttu-id="8bfc5-133">String</span><span class="sxs-lookup"><span data-stu-id="8bfc5-133">String</span></span>     |<span data-ttu-id="8bfc5-134">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-134">Name of the attribute.</span></span> <span data-ttu-id="8bfc5-135">必须是唯一对象定义中。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-135">Must be unique within the object definition.</span></span> <span data-ttu-id="8bfc5-136">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-136">Not nullable.</span></span>|
|<span data-ttu-id="8bfc5-137">必需</span><span class="sxs-lookup"><span data-stu-id="8bfc5-137">required</span></span>       |<span data-ttu-id="8bfc5-138">布尔值</span><span class="sxs-lookup"><span data-stu-id="8bfc5-138">Boolean</span></span>    |<span data-ttu-id="8bfc5-139">`true`如果属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-139">`true` if attribute is required.</span></span> <span data-ttu-id="8bfc5-140">如果缺少任何所需的属性，则不可以创建对象。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-140">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="8bfc5-141">如果同步期间，required 的属性的值，将使用的默认值。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-141">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="8bfc5-142">如果未设置默认值，则同步将记录错误。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-142">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="8bfc5-143">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="8bfc5-143">referencedObjects</span></span>|<span data-ttu-id="8bfc5-144">[referencedObject](../resources/synchronization-referencedobject.md)集合</span><span class="sxs-lookup"><span data-stu-id="8bfc5-144">[referencedObject](../resources/synchronization-referencedobject.md) collection</span></span> |<span data-ttu-id="8bfc5-145">使用属性的`reference`键入，列表被引用的对象 (例如，`manager`属性将列出`User`为引用的对象)。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-145">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="8bfc5-146">type</span><span class="sxs-lookup"><span data-stu-id="8bfc5-146">type</span></span>           |<span data-ttu-id="8bfc5-147">String</span><span class="sxs-lookup"><span data-stu-id="8bfc5-147">String</span></span>     |<span data-ttu-id="8bfc5-148">属性值类型。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-148">Attribute value type.</span></span> <span data-ttu-id="8bfc5-149">可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-149">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="8bfc5-150">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-150">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8bfc5-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bfc5-151">JSON representation</span></span>

<span data-ttu-id="8bfc5-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8bfc5-152">The following is a JSON representation of the resource.</span></span>

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
