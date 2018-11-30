---
title: attributeDefinition 资源类型
description: 描述对象的属性。
ms.openlocfilehash: 2199f8dbe5c528cf3b1b73f007fdae3451833815
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048339"
---
# <a name="attributedefinition-resource-type"></a><span data-ttu-id="76def-103">attributeDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="76def-103">attributeDefinition resource type</span></span>

> <span data-ttu-id="76def-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="76def-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="76def-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="76def-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="76def-106">描述对象的属性。</span><span class="sxs-lookup"><span data-stu-id="76def-106">Describes an attribute of an object.</span></span>

## <a name="properties"></a><span data-ttu-id="76def-107">属性</span><span class="sxs-lookup"><span data-stu-id="76def-107">Properties</span></span>

| <span data-ttu-id="76def-108">属性</span><span class="sxs-lookup"><span data-stu-id="76def-108">Property</span></span>      | <span data-ttu-id="76def-109">类型</span><span class="sxs-lookup"><span data-stu-id="76def-109">Type</span></span>      | <span data-ttu-id="76def-110">说明</span><span class="sxs-lookup"><span data-stu-id="76def-110">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="76def-111">定位</span><span class="sxs-lookup"><span data-stu-id="76def-111">anchor</span></span>         |<span data-ttu-id="76def-112">布尔</span><span class="sxs-lookup"><span data-stu-id="76def-112">Boolean</span></span>    | <span data-ttu-id="76def-113">`true`如果属性应用作对象的定位标记。</span><span class="sxs-lookup"><span data-stu-id="76def-113">`true` if the attribute should be used as the anchor for the object.</span></span> <span data-ttu-id="76def-114">定位属性必须具有识别对象的唯一值，并且必须变。</span><span class="sxs-lookup"><span data-stu-id="76def-114">Anchor attributes must have a unique value identifying an object, and must be immutable.</span></span> <span data-ttu-id="76def-115">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="76def-115">Default is `false`.</span></span> <span data-ttu-id="76def-116">有，并且只有一个对象的属性必须被指定为定位标记为支持同步。</span><span class="sxs-lookup"><span data-stu-id="76def-116">One, and only one, of the object's attributes must be designated as the anchor to support synchronization.</span></span> |
|<span data-ttu-id="76def-117">caseExact</span><span class="sxs-lookup"><span data-stu-id="76def-117">caseExact</span></span>      |<span data-ttu-id="76def-118">布尔</span><span class="sxs-lookup"><span data-stu-id="76def-118">Boolean</span></span>    |<span data-ttu-id="76def-119">`true`如果此属性的值应处理，区分大小写。</span><span class="sxs-lookup"><span data-stu-id="76def-119">`true` if value of this attribute should be treated as case-sensitive.</span></span> <span data-ttu-id="76def-120">此设置会影响如何同步引擎检测到的属性的更改。</span><span class="sxs-lookup"><span data-stu-id="76def-120">This setting affects how the synchronization engine detects changes for the attribute.</span></span>|
|<span data-ttu-id="76def-121">元数据</span><span class="sxs-lookup"><span data-stu-id="76def-121">metadata</span></span>       |[<span data-ttu-id="76def-122">metadataEntry</span><span class="sxs-lookup"><span data-stu-id="76def-122">metadataEntry</span></span>](../resources/synchronization-metadataentry.md)    |<span data-ttu-id="76def-123">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="76def-123">Additional extension properties.</span></span> <span data-ttu-id="76def-124">除非明确提到，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="76def-124">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="76def-125">多值</span><span class="sxs-lookup"><span data-stu-id="76def-125">multivalued</span></span>    |<span data-ttu-id="76def-126">布尔</span><span class="sxs-lookup"><span data-stu-id="76def-126">Boolean</span></span>    |<span data-ttu-id="76def-127">`true`如果属性可以有多个值。</span><span class="sxs-lookup"><span data-stu-id="76def-127">`true` if an attribute can have multiple values.</span></span> <span data-ttu-id="76def-128">默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="76def-128">Default is `false`.</span></span>|
|<span data-ttu-id="76def-129">mutability</span><span class="sxs-lookup"><span data-stu-id="76def-129">mutability</span></span>     |<span data-ttu-id="76def-130">字符串</span><span class="sxs-lookup"><span data-stu-id="76def-130">String</span></span>     |<span data-ttu-id="76def-131">属性可变性。</span><span class="sxs-lookup"><span data-stu-id="76def-131">An attribute's mutability.</span></span> <span data-ttu-id="76def-132">可能的值为： `ReadWrite`， `ReadOnly`， `Immutable`， `WriteOnly`。</span><span class="sxs-lookup"><span data-stu-id="76def-132">Possible values are:  `ReadWrite`, `ReadOnly`, `Immutable`, `WriteOnly`.</span></span> <span data-ttu-id="76def-133">默认值为 `ReadWrite`。</span><span class="sxs-lookup"><span data-stu-id="76def-133">Default is `ReadWrite`.</span></span>|
|<span data-ttu-id="76def-134">name</span><span class="sxs-lookup"><span data-stu-id="76def-134">name</span></span>           |<span data-ttu-id="76def-135">字符串</span><span class="sxs-lookup"><span data-stu-id="76def-135">String</span></span>     |<span data-ttu-id="76def-136">属性的名称。</span><span class="sxs-lookup"><span data-stu-id="76def-136">Name of the attribute.</span></span> <span data-ttu-id="76def-137">必须是唯一对象定义中。</span><span class="sxs-lookup"><span data-stu-id="76def-137">Must be unique within the object definition.</span></span> <span data-ttu-id="76def-138">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="76def-138">Not nullable.</span></span>|
|<span data-ttu-id="76def-139">必需</span><span class="sxs-lookup"><span data-stu-id="76def-139">required</span></span>       |<span data-ttu-id="76def-140">布尔</span><span class="sxs-lookup"><span data-stu-id="76def-140">Boolean</span></span>    |<span data-ttu-id="76def-141">`true`如果属性是必需的。</span><span class="sxs-lookup"><span data-stu-id="76def-141">`true` if attribute is required.</span></span> <span data-ttu-id="76def-142">如果缺少任何所需的属性，则不可以创建对象。</span><span class="sxs-lookup"><span data-stu-id="76def-142">Object can not be created if any of the required attributes are missing.</span></span> <span data-ttu-id="76def-143">如果同步期间，required 的属性的值，将使用的默认值。</span><span class="sxs-lookup"><span data-stu-id="76def-143">If during synchronization, the required attribute has no value, the default value will be used.</span></span> <span data-ttu-id="76def-144">如果未设置默认值，则同步将记录错误。</span><span class="sxs-lookup"><span data-stu-id="76def-144">If default the value was not set, synchronization will record an error.</span></span>|
|<span data-ttu-id="76def-145">referencedObjects</span><span class="sxs-lookup"><span data-stu-id="76def-145">referencedObjects</span></span>|[<span data-ttu-id="76def-146">referencedObject</span><span class="sxs-lookup"><span data-stu-id="76def-146">referencedObject</span></span>](../resources/synchronization-referencedobject.md) |<span data-ttu-id="76def-147">使用属性的`reference`键入，列表被引用的对象 (例如，`manager`属性将列出`User`为引用的对象)。</span><span class="sxs-lookup"><span data-stu-id="76def-147">For attributes with `reference` type, lists referenced objects (for example, the `manager` attribute would list `User` as the referenced object).</span></span>|
|<span data-ttu-id="76def-148">type</span><span class="sxs-lookup"><span data-stu-id="76def-148">type</span></span>           |<span data-ttu-id="76def-149">字符串</span><span class="sxs-lookup"><span data-stu-id="76def-149">String</span></span>     |<span data-ttu-id="76def-150">属性值类型。</span><span class="sxs-lookup"><span data-stu-id="76def-150">Attribute value type.</span></span> <span data-ttu-id="76def-151">可取值为：`String`、`Integer`、`Reference`、`Binary` 或 `Boolean`。</span><span class="sxs-lookup"><span data-stu-id="76def-151">Possible values are: `String`, `Integer`, `Reference`, `Binary`, `Boolean`.</span></span> <span data-ttu-id="76def-152">默认值为 `String`。</span><span class="sxs-lookup"><span data-stu-id="76def-152">Default is `String`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76def-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76def-153">JSON representation</span></span>

<span data-ttu-id="76def-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76def-154">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "attributeDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->