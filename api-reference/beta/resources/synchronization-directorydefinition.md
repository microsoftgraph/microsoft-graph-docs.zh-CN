---
title: directoryDefinition 资源类型
description: 提供有关目录及其对象的同步引擎信息。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: cb0eb46feebb743a30593bf6e1d2b0142077cc7e
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718449"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="cec00-103">directoryDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="cec00-103">directoryDefinition resource type</span></span>

<span data-ttu-id="cec00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cec00-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cec00-105">提供有关目录及其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="cec00-105">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="cec00-106">例如，此资源告知同步引擎，该目录具有名为 user 和 **group** 的对象、这些对象支持哪些属性以及这些属性的类型。</span><span class="sxs-lookup"><span data-stu-id="cec00-106">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="cec00-107">为了使对象和属性参与同步[规则和](synchronization-synchronizationrule.md)[对象](synchronization-objectmapping.md)映射，必须将它们定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="cec00-107">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="cec00-108">通常[，作为同步](synchronization-synchronizationschema.md)模板的一部分提供的默认同步架构[](synchronization-synchronizationtemplate.md)将定义该目录最常用的对象和属性。</span><span class="sxs-lookup"><span data-stu-id="cec00-108">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="cec00-109">但是，如果目录支持添加自定义属性，您可能需要使用自己的自定义对象或属性扩展默认定义。</span><span class="sxs-lookup"><span data-stu-id="cec00-109">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="cec00-110">有关详细信息，请参阅配置[与自定义属性的同步以及](synchronization-configure-with-custom-target-attributes.md)[配置与目录扩展属性的同步](synchronization-configure-with-directory-extension-attributes.md)。</span><span class="sxs-lookup"><span data-stu-id="cec00-110">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="cec00-111">目录定义作为同步架构的一 [部分进行更新](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="cec00-111">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="cec00-112">方法</span><span class="sxs-lookup"><span data-stu-id="cec00-112">Methods</span></span>

| <span data-ttu-id="cec00-113">方法</span><span class="sxs-lookup"><span data-stu-id="cec00-113">Method</span></span>       | <span data-ttu-id="cec00-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="cec00-114">Return Type</span></span>  |<span data-ttu-id="cec00-115">说明</span><span class="sxs-lookup"><span data-stu-id="cec00-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cec00-116">发现 directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="cec00-116">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="cec00-117">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="cec00-117">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="cec00-118">发现目录的架构和支持的属性。</span><span class="sxs-lookup"><span data-stu-id="cec00-118">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="cec00-119">属性</span><span class="sxs-lookup"><span data-stu-id="cec00-119">Properties</span></span>

| <span data-ttu-id="cec00-120">属性</span><span class="sxs-lookup"><span data-stu-id="cec00-120">Property</span></span>      | <span data-ttu-id="cec00-121">类型</span><span class="sxs-lookup"><span data-stu-id="cec00-121">Type</span></span>      | <span data-ttu-id="cec00-122">说明</span><span class="sxs-lookup"><span data-stu-id="cec00-122">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="cec00-123">id</span><span class="sxs-lookup"><span data-stu-id="cec00-123">id</span></span>           |<span data-ttu-id="cec00-124">String</span><span class="sxs-lookup"><span data-stu-id="cec00-124">String</span></span>     |<span data-ttu-id="cec00-125">目录标识符。</span><span class="sxs-lookup"><span data-stu-id="cec00-125">Directory identifier.</span></span> <span data-ttu-id="cec00-126">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="cec00-126">Not nullable.</span></span>|
|<span data-ttu-id="cec00-127">元数据</span><span class="sxs-lookup"><span data-stu-id="cec00-127">metadata</span></span>       |<span data-ttu-id="cec00-128">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="cec00-128">metadataEntry collection</span></span>    |<span data-ttu-id="cec00-129">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="cec00-129">Additional extension properties.</span></span> <span data-ttu-id="cec00-130">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="cec00-130">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="cec00-131">name</span><span class="sxs-lookup"><span data-stu-id="cec00-131">name</span></span>           |<span data-ttu-id="cec00-132">String</span><span class="sxs-lookup"><span data-stu-id="cec00-132">String</span></span>     |<span data-ttu-id="cec00-133">目录的名称。</span><span class="sxs-lookup"><span data-stu-id="cec00-133">Name of the directory.</span></span> <span data-ttu-id="cec00-134">在同步架构中 [必须是唯一的](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="cec00-134">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="cec00-135">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="cec00-135">Not nullable.</span></span>|
|<span data-ttu-id="cec00-136">对象</span><span class="sxs-lookup"><span data-stu-id="cec00-136">objects</span></span>        |<span data-ttu-id="cec00-137">[objectDefinition](synchronization-objectdefinition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cec00-137">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="cec00-138">目录支持的对象的集合。</span><span class="sxs-lookup"><span data-stu-id="cec00-138">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="cec00-139">version</span><span class="sxs-lookup"><span data-stu-id="cec00-139">version</span></span>|<span data-ttu-id="cec00-140">String</span><span class="sxs-lookup"><span data-stu-id="cec00-140">String</span></span>|<span data-ttu-id="cec00-141">指示发现的版本的只读值。</span><span class="sxs-lookup"><span data-stu-id="cec00-141">Read only value that indicates version discovered.</span></span> <span data-ttu-id="cec00-142">如果尚未发现，则其为 Null。</span><span class="sxs-lookup"><span data-stu-id="cec00-142">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="cec00-143">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="cec00-143">discoveryDateTime</span></span>|<span data-ttu-id="cec00-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cec00-144">DateTimeOffset</span></span>| <span data-ttu-id="cec00-145">表示使用 ISO 8601 格式的发现日期和时间，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="cec00-145">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="cec00-146">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="cec00-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="cec00-147">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="cec00-147">discoverabilities</span></span>|<span data-ttu-id="cec00-148">string</span><span class="sxs-lookup"><span data-stu-id="cec00-148">string</span></span>| <span data-ttu-id="cec00-149">只读值，指示应用支持哪种类型的发现。</span><span class="sxs-lookup"><span data-stu-id="cec00-149">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="cec00-150">可取值为：`AttributeDataTypes`、`AttributeNames`、`AttributeReadOnly`、`None`、`ReferenceAttributes`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="cec00-150">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="cec00-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cec00-151">JSON representation</span></span>

<span data-ttu-id="cec00-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cec00-152">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directoryDefinition"
}-->

```json
{
  "discoverabilities": "String",
  "discoveryDateTime": "DateTimeOffset",
  "id": "String",
  "metadata": [{"@odata.type": "microsoft.graph.stringKeyStringValuePair"}],
  "name": "String",
  "objects": [{"@odata.type": "microsoft.graph.objectDefinition"}],
  "version": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryDefinition resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


