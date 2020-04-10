---
title: synchronizationTemplate 资源类型
description: 为特定应用程序提供预先配置的同步设置。
localization_priority: Normal
doc_type: resourcePageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5067df26f0b1c1e6b77d1c3d87d4c73bb9e45208
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43217001"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="ef04f-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="ef04f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ef04f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ef04f-105">为特定应用程序提供预先配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="ef04f-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="ef04f-106">默认情况下，将对基于该模板的任何[同步作业](synchronization-synchronizationjob.md)使用这些设置。</span><span class="sxs-lookup"><span data-stu-id="ef04f-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="ef04f-107">应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置，包括[同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="ef04f-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="ef04f-108">您可以为应用程序提供多个模板，并指定一个默认模板。</span><span class="sxs-lookup"><span data-stu-id="ef04f-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="ef04f-109">如果有多个模板可用于您感兴趣的应用程序，请查找特定于应用程序的指南，以确定哪一个模板最符合您的需求。</span><span class="sxs-lookup"><span data-stu-id="ef04f-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="ef04f-110">Methods</span><span class="sxs-lookup"><span data-stu-id="ef04f-110">Methods</span></span>

| <span data-ttu-id="ef04f-111">方法</span><span class="sxs-lookup"><span data-stu-id="ef04f-111">Method</span></span>        | <span data-ttu-id="ef04f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-112">Return Type</span></span>               | <span data-ttu-id="ef04f-113">说明</span><span class="sxs-lookup"><span data-stu-id="ef04f-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="ef04f-114">List</span><span class="sxs-lookup"><span data-stu-id="ef04f-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="ef04f-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="ef04f-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="ef04f-116">列出可用于应用程序实例或应用程序实例（服务主体）的模板。</span><span class="sxs-lookup"><span data-stu-id="ef04f-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="ef04f-117">获取</span><span class="sxs-lookup"><span data-stu-id="ef04f-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="ef04f-118">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="ef04f-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="ef04f-119">读取**synchronizationTemplate**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ef04f-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="ef04f-120">属性</span><span class="sxs-lookup"><span data-stu-id="ef04f-120">Properties</span></span>

| <span data-ttu-id="ef04f-121">属性</span><span class="sxs-lookup"><span data-stu-id="ef04f-121">Property</span></span>      | <span data-ttu-id="ef04f-122">类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-122">Type</span></span>                      | <span data-ttu-id="ef04f-123">Description</span><span class="sxs-lookup"><span data-stu-id="ef04f-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="ef04f-124">id</span><span class="sxs-lookup"><span data-stu-id="ef04f-124">id</span></span>             |<span data-ttu-id="ef04f-125">字符串</span><span class="sxs-lookup"><span data-stu-id="ef04f-125">String</span></span>                     |<span data-ttu-id="ef04f-126">唯一的模板标识符。</span><span class="sxs-lookup"><span data-stu-id="ef04f-126">Unique template identifier.</span></span>|
|<span data-ttu-id="ef04f-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="ef04f-127">applicationId</span></span>  |<span data-ttu-id="ef04f-128">String</span><span class="sxs-lookup"><span data-stu-id="ef04f-128">String</span></span>                     |<span data-ttu-id="ef04f-129">此模板所属应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="ef04f-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="ef04f-130">设置</span><span class="sxs-lookup"><span data-stu-id="ef04f-130">default</span></span>        |<span data-ttu-id="ef04f-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="ef04f-131">Boolean</span></span>                    |<span data-ttu-id="ef04f-132">`true`如果建议将此模板作为应用程序的默认模板。</span><span class="sxs-lookup"><span data-stu-id="ef04f-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="ef04f-133">说明</span><span class="sxs-lookup"><span data-stu-id="ef04f-133">description</span></span>    |<span data-ttu-id="ef04f-134">String</span><span class="sxs-lookup"><span data-stu-id="ef04f-134">String</span></span>                     |<span data-ttu-id="ef04f-135">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="ef04f-135">Description of the template.</span></span>|
|<span data-ttu-id="ef04f-136">被</span><span class="sxs-lookup"><span data-stu-id="ef04f-136">discoverable</span></span>   |<span data-ttu-id="ef04f-137">字符串</span><span class="sxs-lookup"><span data-stu-id="ef04f-137">String</span></span>                     |<span data-ttu-id="ef04f-138">`true`如果此模板应显示在可用于应用程序实例（服务主体）的模板集合中。</span><span class="sxs-lookup"><span data-stu-id="ef04f-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="ef04f-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="ef04f-139">factoryTag</span></span>     |<span data-ttu-id="ef04f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="ef04f-140">String</span></span>                     |<span data-ttu-id="ef04f-141">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="ef04f-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="ef04f-142">**FactoryTag**告知同步引擎在处理基于此模板的作业时要使用的实现。</span><span class="sxs-lookup"><span data-stu-id="ef04f-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="ef04f-143">metadata</span><span class="sxs-lookup"><span data-stu-id="ef04f-143">metadata</span></span>       |<span data-ttu-id="ef04f-144">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="ef04f-144">metadataEntry collection</span></span>   |<span data-ttu-id="ef04f-145">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="ef04f-145">Additional extension properties.</span></span> <span data-ttu-id="ef04f-146">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="ef04f-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ef04f-147">关系</span><span class="sxs-lookup"><span data-stu-id="ef04f-147">Relationships</span></span>
| <span data-ttu-id="ef04f-148">关系</span><span class="sxs-lookup"><span data-stu-id="ef04f-148">Relationship</span></span>      | <span data-ttu-id="ef04f-149">类型</span><span class="sxs-lookup"><span data-stu-id="ef04f-149">Type</span></span>      |<span data-ttu-id="ef04f-150">Description</span><span class="sxs-lookup"><span data-stu-id="ef04f-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="ef04f-151">架构</span><span class="sxs-lookup"><span data-stu-id="ef04f-151">schema</span></span>             |[<span data-ttu-id="ef04f-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="ef04f-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="ef04f-153">基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="ef04f-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef04f-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ef04f-154">JSON representation</span></span>

<span data-ttu-id="ef04f-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef04f-155">The following is a JSON representation of the resource.</span></span>

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
