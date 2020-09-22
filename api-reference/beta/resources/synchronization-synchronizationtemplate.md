---
title: synchronizationTemplate 资源类型
description: 为特定应用程序提供预先配置的同步设置。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d794391c4cf8043ab4eaeafcfa21958d93e3412a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985683"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="c8d60-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8d60-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="c8d60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8d60-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8d60-105">为特定应用程序提供预先配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="c8d60-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="c8d60-106">默认情况下，将对基于该模板的任何 [同步作业](synchronization-synchronizationjob.md) 使用这些设置。</span><span class="sxs-lookup"><span data-stu-id="c8d60-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="c8d60-107">应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置，包括 [同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="c8d60-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="c8d60-108">您可以为应用程序提供多个模板，并指定一个默认模板。</span><span class="sxs-lookup"><span data-stu-id="c8d60-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="c8d60-109">如果有多个模板可用于您感兴趣的应用程序，请查找特定于应用程序的指南，以确定哪一个模板最符合您的需求。</span><span class="sxs-lookup"><span data-stu-id="c8d60-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="c8d60-110">方法</span><span class="sxs-lookup"><span data-stu-id="c8d60-110">Methods</span></span>

| <span data-ttu-id="c8d60-111">方法</span><span class="sxs-lookup"><span data-stu-id="c8d60-111">Method</span></span>        | <span data-ttu-id="c8d60-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8d60-112">Return Type</span></span>               | <span data-ttu-id="c8d60-113">Description</span><span class="sxs-lookup"><span data-stu-id="c8d60-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="c8d60-114">List</span><span class="sxs-lookup"><span data-stu-id="c8d60-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="c8d60-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8d60-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="c8d60-116">列出 (服务主体) 的应用程序或应用程序实例可用的模板。</span><span class="sxs-lookup"><span data-stu-id="c8d60-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="c8d60-117">获取</span><span class="sxs-lookup"><span data-stu-id="c8d60-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="c8d60-118">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="c8d60-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="c8d60-119">读取 **synchronizationTemplate** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8d60-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="c8d60-120">属性</span><span class="sxs-lookup"><span data-stu-id="c8d60-120">Properties</span></span>

| <span data-ttu-id="c8d60-121">属性</span><span class="sxs-lookup"><span data-stu-id="c8d60-121">Property</span></span>      | <span data-ttu-id="c8d60-122">类型</span><span class="sxs-lookup"><span data-stu-id="c8d60-122">Type</span></span>                      | <span data-ttu-id="c8d60-123">说明</span><span class="sxs-lookup"><span data-stu-id="c8d60-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="c8d60-124">id</span><span class="sxs-lookup"><span data-stu-id="c8d60-124">id</span></span>             |<span data-ttu-id="c8d60-125">String</span><span class="sxs-lookup"><span data-stu-id="c8d60-125">String</span></span>                     |<span data-ttu-id="c8d60-126">唯一的模板标识符。</span><span class="sxs-lookup"><span data-stu-id="c8d60-126">Unique template identifier.</span></span>|
|<span data-ttu-id="c8d60-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="c8d60-127">applicationId</span></span>  |<span data-ttu-id="c8d60-128">String</span><span class="sxs-lookup"><span data-stu-id="c8d60-128">String</span></span>                     |<span data-ttu-id="c8d60-129">此模板所属应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="c8d60-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="c8d60-130">设置</span><span class="sxs-lookup"><span data-stu-id="c8d60-130">default</span></span>        |<span data-ttu-id="c8d60-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8d60-131">Boolean</span></span>                    |<span data-ttu-id="c8d60-132">`true` 如果建议将此模板作为应用程序的默认模板。</span><span class="sxs-lookup"><span data-stu-id="c8d60-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="c8d60-133">description</span><span class="sxs-lookup"><span data-stu-id="c8d60-133">description</span></span>    |<span data-ttu-id="c8d60-134">String</span><span class="sxs-lookup"><span data-stu-id="c8d60-134">String</span></span>                     |<span data-ttu-id="c8d60-135">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="c8d60-135">Description of the template.</span></span>|
|<span data-ttu-id="c8d60-136">被</span><span class="sxs-lookup"><span data-stu-id="c8d60-136">discoverable</span></span>   |<span data-ttu-id="c8d60-137">String</span><span class="sxs-lookup"><span data-stu-id="c8d60-137">String</span></span>                     |<span data-ttu-id="c8d60-138">`true` 如果此模板应显示在应用程序实例的可用模板集合中 (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="c8d60-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="c8d60-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="c8d60-139">factoryTag</span></span>     |<span data-ttu-id="c8d60-140">String</span><span class="sxs-lookup"><span data-stu-id="c8d60-140">String</span></span>                     |<span data-ttu-id="c8d60-141">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="c8d60-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="c8d60-142">**FactoryTag**告知同步引擎在处理基于此模板的作业时要使用的实现。</span><span class="sxs-lookup"><span data-stu-id="c8d60-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="c8d60-143">metadata</span><span class="sxs-lookup"><span data-stu-id="c8d60-143">metadata</span></span>       |<span data-ttu-id="c8d60-144">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="c8d60-144">metadataEntry collection</span></span>   |<span data-ttu-id="c8d60-145">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c8d60-145">Additional extension properties.</span></span> <span data-ttu-id="c8d60-146">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="c8d60-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8d60-147">关系</span><span class="sxs-lookup"><span data-stu-id="c8d60-147">Relationships</span></span>
| <span data-ttu-id="c8d60-148">关系</span><span class="sxs-lookup"><span data-stu-id="c8d60-148">Relationship</span></span>      | <span data-ttu-id="c8d60-149">类型</span><span class="sxs-lookup"><span data-stu-id="c8d60-149">Type</span></span>      |<span data-ttu-id="c8d60-150">说明</span><span class="sxs-lookup"><span data-stu-id="c8d60-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="c8d60-151">架构</span><span class="sxs-lookup"><span data-stu-id="c8d60-151">schema</span></span>             |[<span data-ttu-id="c8d60-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="c8d60-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="c8d60-153">基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="c8d60-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c8d60-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8d60-154">JSON representation</span></span>

<span data-ttu-id="c8d60-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8d60-155">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.synchronizationTemplate"
}-->

```json
{
  "applicationId": "String (identifier)",
  "default": true,
  "description": "String",
  "discoverable": true,
  "factoryTag": "String",
  "id": "String (identifier)",
  "metadata": [{"@odata.type": "microsoft.graph.metadataEntry"}],
  "schema": {"@odata.type": "microsoft.graph.synchronizationSchema"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


