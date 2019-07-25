---
title: directoryDefinition 资源类型
description: 提供有关目录及其对象的同步引擎信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 56c1f5a6a15f7ab6724feff68aa38eba1ef22694
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888137"
---
# <a name="directorydefinition-resource-type"></a><span data-ttu-id="d8f9e-103">directoryDefinition 资源类型</span><span class="sxs-lookup"><span data-stu-id="d8f9e-103">directoryDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8f9e-104">提供有关目录及其对象的同步引擎信息。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-104">Provides the synchronization engine information about a directory and its objects.</span></span> <span data-ttu-id="d8f9e-105">此资源将告知同步引擎, 例如, 目录包含名为**user**和**group**的对象、支持这些对象的属性以及这些属性的类型。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-105">This resource tells the synchronization engine, for example, that the directory has objects named **user** and **group**, which attributes are supported for those objects, and the types for those attributes.</span></span> <span data-ttu-id="d8f9e-106">为了使对象和属性参与[同步规则](synchronization-synchronizationrule.md)和[对象映射](synchronization-objectmapping.md), 必须将它们定义为目录定义的一部分。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-106">In order for the object and attribute to participate in [synchronization rules](synchronization-synchronizationrule.md) and [object mappings](synchronization-objectmapping.md), they must be defined as part of the directory definition.</span></span>

<span data-ttu-id="d8f9e-107">通常, 作为[同步模板](synchronization-synchronizationtemplate.md)的一部分提供的默认[同步架构](synchronization-synchronizationschema.md)将为该目录定义最常用的对象和属性。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-107">In general, the default [synchronization schema](synchronization-synchronizationschema.md) provided as part of the [synchronization template](synchronization-synchronizationtemplate.md) will define most commonly used objects and attributes for that directory.</span></span> <span data-ttu-id="d8f9e-108">但是, 如果目录支持添加自定义属性, 则可能需要使用自己的自定义对象或属性扩展默认定义。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-108">However, if the directory supports the addition of custom attributes, you might want to expand the default definition with your own custom objects or attributes.</span></span> <span data-ttu-id="d8f9e-109">有关详细信息, 请参阅[配置与自定义属性的同步](synchronization-configure-with-custom-target-attributes.md)和[配置与目录扩展属性的同步](synchronization-configure-with-directory-extension-attributes.md)。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-109">For more information, see [Configure synchronization with custom attributes](synchronization-configure-with-custom-target-attributes.md) and [Configure synchronization with directory extension attributes](synchronization-configure-with-directory-extension-attributes.md).</span></span>

<span data-ttu-id="d8f9e-110">目录定义作为[同步架构](synchronization-synchronizationschema.md)的一部分进行更新。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-110">Directory definitions are updated as part of the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d8f9e-111">方法</span><span class="sxs-lookup"><span data-stu-id="d8f9e-111">Methods</span></span>

| <span data-ttu-id="d8f9e-112">方法</span><span class="sxs-lookup"><span data-stu-id="d8f9e-112">Method</span></span>       | <span data-ttu-id="d8f9e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="d8f9e-113">Return Type</span></span>  |<span data-ttu-id="d8f9e-114">说明</span><span class="sxs-lookup"><span data-stu-id="d8f9e-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d8f9e-115">发现 directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="d8f9e-115">Discover directoryDefinition</span></span>](../api/directorydefinition-discover.md) | [<span data-ttu-id="d8f9e-116">directoryDefinition</span><span class="sxs-lookup"><span data-stu-id="d8f9e-116">directoryDefinition</span></span>](synchronization-directorydefinition.md) |<span data-ttu-id="d8f9e-117">发现目录的架构和受支持的属性。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-117">Discover the schema and supported properties of the directory.</span></span>|

## <a name="properties"></a><span data-ttu-id="d8f9e-118">属性</span><span class="sxs-lookup"><span data-stu-id="d8f9e-118">Properties</span></span>

| <span data-ttu-id="d8f9e-119">属性</span><span class="sxs-lookup"><span data-stu-id="d8f9e-119">Property</span></span>      | <span data-ttu-id="d8f9e-120">类型</span><span class="sxs-lookup"><span data-stu-id="d8f9e-120">Type</span></span>      | <span data-ttu-id="d8f9e-121">说明</span><span class="sxs-lookup"><span data-stu-id="d8f9e-121">Description</span></span>    |
|:--------------|:----------|:---------------|
|<span data-ttu-id="d8f9e-122">id</span><span class="sxs-lookup"><span data-stu-id="d8f9e-122">id</span></span>           |<span data-ttu-id="d8f9e-123">String</span><span class="sxs-lookup"><span data-stu-id="d8f9e-123">String</span></span>     |<span data-ttu-id="d8f9e-124">目录标识符。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-124">Directory identifier.</span></span> <span data-ttu-id="d8f9e-125">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-125">Not nullable.</span></span>|
|<span data-ttu-id="d8f9e-126">metadata</span><span class="sxs-lookup"><span data-stu-id="d8f9e-126">metadata</span></span>       |<span data-ttu-id="d8f9e-127">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="d8f9e-127">metadataEntry collection</span></span>    |<span data-ttu-id="d8f9e-128">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-128">Additional extension properties.</span></span> <span data-ttu-id="d8f9e-129">除非明确提到, 否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-129">Unless mentioned explicitly, metadata values should not be changed.</span></span>|
|<span data-ttu-id="d8f9e-130">name</span><span class="sxs-lookup"><span data-stu-id="d8f9e-130">name</span></span>           |<span data-ttu-id="d8f9e-131">String</span><span class="sxs-lookup"><span data-stu-id="d8f9e-131">String</span></span>     |<span data-ttu-id="d8f9e-132">目录的名称。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-132">Name of the directory.</span></span> <span data-ttu-id="d8f9e-133">在[同步架构](synchronization-synchronizationschema.md)中必须是唯一的。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-133">Must be unique within the [synchronization schema](synchronization-synchronizationschema.md).</span></span> <span data-ttu-id="d8f9e-134">不可为 null。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-134">Not nullable.</span></span>|
|<span data-ttu-id="d8f9e-135">对象</span><span class="sxs-lookup"><span data-stu-id="d8f9e-135">objects</span></span>        |<span data-ttu-id="d8f9e-136">[objectDefinition](synchronization-objectdefinition.md)集合</span><span class="sxs-lookup"><span data-stu-id="d8f9e-136">[objectDefinition](synchronization-objectdefinition.md) collection</span></span>    |<span data-ttu-id="d8f9e-137">目录支持的对象集合。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-137">Collection of objects supported by the directory.</span></span>|
|<span data-ttu-id="d8f9e-138">version</span><span class="sxs-lookup"><span data-stu-id="d8f9e-138">version</span></span>|<span data-ttu-id="d8f9e-139">String</span><span class="sxs-lookup"><span data-stu-id="d8f9e-139">String</span></span>|<span data-ttu-id="d8f9e-140">只读值, 指示发现的版本。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-140">Read only value that indicates version discovered.</span></span> <span data-ttu-id="d8f9e-141">如果尚未发生发现, 则为 Null。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-141">Null if discovery has not yet occurred.</span></span>|
|<span data-ttu-id="d8f9e-142">discoveryDateTime</span><span class="sxs-lookup"><span data-stu-id="d8f9e-142">discoveryDateTime</span></span>|<span data-ttu-id="d8f9e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8f9e-143">DateTimeOffset</span></span>| <span data-ttu-id="d8f9e-144">表示使用 ISO 8601 格式的发现日期和时间, 并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-144">Represents the discovery date and time using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d8f9e-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="d8f9e-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="d8f9e-146">discoverabilities</span><span class="sxs-lookup"><span data-stu-id="d8f9e-146">discoverabilities</span></span>|<span data-ttu-id="d8f9e-147">string</span><span class="sxs-lookup"><span data-stu-id="d8f9e-147">string</span></span>| <span data-ttu-id="d8f9e-148">只读指示应用程序支持的发现类型的值。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-148">Read only value indicating what type of discovery the app supports.</span></span> <span data-ttu-id="d8f9e-149">可取值为：`AttributeDataTypes`、`AttributeNames`、`AttributeReadOnly`、`None`、`ReferenceAttributes`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-149">Possible values are: `AttributeDataTypes`, `AttributeNames`, `AttributeReadOnly`, `None`, `ReferenceAttributes`, `UnknownFutureValue`.</span></span>| 

## <a name="json-representation"></a><span data-ttu-id="d8f9e-150">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d8f9e-150">JSON representation</span></span>

<span data-ttu-id="d8f9e-151">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8f9e-151">The following is a JSON representation of the resource.</span></span>

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
