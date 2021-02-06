---
title: synchronizationTemplate 资源类型
description: 为特定应用程序提供预配置的同步设置。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: c08f5c3eee6225a1149ff993415f83b2e5916583
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132298"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="61a6a-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="61a6a-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="61a6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61a6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="61a6a-105">为特定应用程序提供预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="61a6a-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="61a6a-106">默认情况下，这些设置将用于基于模板的任何同步作业[](synchronization-synchronizationjob.md)。</span><span class="sxs-lookup"><span data-stu-id="61a6a-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="61a6a-107">应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置，包括 [同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="61a6a-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="61a6a-108">可以为应用程序提供多个模板，并指定默认模板。</span><span class="sxs-lookup"><span data-stu-id="61a6a-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="61a6a-109">如果对感兴趣的应用程序提供了多个模板，请寻找特定于应用程序的指南，以确定哪个模板最能满足你的需求。</span><span class="sxs-lookup"><span data-stu-id="61a6a-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="61a6a-110">方法</span><span class="sxs-lookup"><span data-stu-id="61a6a-110">Methods</span></span>

| <span data-ttu-id="61a6a-111">方法</span><span class="sxs-lookup"><span data-stu-id="61a6a-111">Method</span></span>        | <span data-ttu-id="61a6a-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="61a6a-112">Return Type</span></span>               | <span data-ttu-id="61a6a-113">Description</span><span class="sxs-lookup"><span data-stu-id="61a6a-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="61a6a-114">List</span><span class="sxs-lookup"><span data-stu-id="61a6a-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="61a6a-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="61a6a-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="61a6a-116">列出可用于应用程序或应用程序实例的模板 (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="61a6a-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="61a6a-117">获取</span><span class="sxs-lookup"><span data-stu-id="61a6a-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="61a6a-118">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="61a6a-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="61a6a-119">读取 **synchronizationTemplate** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="61a6a-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="61a6a-120">属性</span><span class="sxs-lookup"><span data-stu-id="61a6a-120">Properties</span></span>

| <span data-ttu-id="61a6a-121">属性</span><span class="sxs-lookup"><span data-stu-id="61a6a-121">Property</span></span>      | <span data-ttu-id="61a6a-122">类型</span><span class="sxs-lookup"><span data-stu-id="61a6a-122">Type</span></span>                      | <span data-ttu-id="61a6a-123">说明</span><span class="sxs-lookup"><span data-stu-id="61a6a-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="61a6a-124">id</span><span class="sxs-lookup"><span data-stu-id="61a6a-124">id</span></span>             |<span data-ttu-id="61a6a-125">字符串</span><span class="sxs-lookup"><span data-stu-id="61a6a-125">String</span></span>                     |<span data-ttu-id="61a6a-126">唯一模板标识符。</span><span class="sxs-lookup"><span data-stu-id="61a6a-126">Unique template identifier.</span></span>|
|<span data-ttu-id="61a6a-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="61a6a-127">applicationId</span></span>  |<span data-ttu-id="61a6a-128">String</span><span class="sxs-lookup"><span data-stu-id="61a6a-128">String</span></span>                     |<span data-ttu-id="61a6a-129">此模板所属的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="61a6a-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="61a6a-130"> 默认值</span><span class="sxs-lookup"><span data-stu-id="61a6a-130">default</span></span>        |<span data-ttu-id="61a6a-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="61a6a-131">Boolean</span></span>                    |<span data-ttu-id="61a6a-132">`true` 如果建议此模板为应用程序的默认值。</span><span class="sxs-lookup"><span data-stu-id="61a6a-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="61a6a-133">说明</span><span class="sxs-lookup"><span data-stu-id="61a6a-133">description</span></span>    |<span data-ttu-id="61a6a-134">字符串</span><span class="sxs-lookup"><span data-stu-id="61a6a-134">String</span></span>                     |<span data-ttu-id="61a6a-135">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="61a6a-135">Description of the template.</span></span>|
|<span data-ttu-id="61a6a-136">可发现</span><span class="sxs-lookup"><span data-stu-id="61a6a-136">discoverable</span></span>   |<span data-ttu-id="61a6a-137">字符串</span><span class="sxs-lookup"><span data-stu-id="61a6a-137">String</span></span>                     |<span data-ttu-id="61a6a-138">`true` 如果此模板应显示在可用于应用程序实例的模板集合中， (服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="61a6a-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="61a6a-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="61a6a-139">factoryTag</span></span>     |<span data-ttu-id="61a6a-140">字符串</span><span class="sxs-lookup"><span data-stu-id="61a6a-140">String</span></span>                     |<span data-ttu-id="61a6a-141">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="61a6a-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="61a6a-142">**factoryTag** 告知同步引擎在基于此模板处理作业时要使用哪种实现。</span><span class="sxs-lookup"><span data-stu-id="61a6a-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="61a6a-143">metadata</span><span class="sxs-lookup"><span data-stu-id="61a6a-143">metadata</span></span>       |<span data-ttu-id="61a6a-144">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="61a6a-144">metadataEntry collection</span></span>   |<span data-ttu-id="61a6a-145">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="61a6a-145">Additional extension properties.</span></span> <span data-ttu-id="61a6a-146">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="61a6a-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="61a6a-147">关系</span><span class="sxs-lookup"><span data-stu-id="61a6a-147">Relationships</span></span>
| <span data-ttu-id="61a6a-148">关系</span><span class="sxs-lookup"><span data-stu-id="61a6a-148">Relationship</span></span>      | <span data-ttu-id="61a6a-149">类型</span><span class="sxs-lookup"><span data-stu-id="61a6a-149">Type</span></span>      |<span data-ttu-id="61a6a-150">说明</span><span class="sxs-lookup"><span data-stu-id="61a6a-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="61a6a-151">架构</span><span class="sxs-lookup"><span data-stu-id="61a6a-151">schema</span></span>             |[<span data-ttu-id="61a6a-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="61a6a-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="61a6a-153">基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="61a6a-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61a6a-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61a6a-154">JSON representation</span></span>

<span data-ttu-id="61a6a-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61a6a-155">The following is a JSON representation of the resource.</span></span>

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


