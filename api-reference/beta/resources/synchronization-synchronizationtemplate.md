---
title: synchronizationTemplate 资源类型
description: " 任何人都可以检索要查看默认设置，包括同步架构的模板。"
localization_priority: Normal
ms.openlocfilehash: e98d3fa16d0a80ac9353aaa75200d8cb24d3e904
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833073"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="fde17-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="fde17-103">synchronizationTemplate resource type</span></span>

> <span data-ttu-id="fde17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fde17-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fde17-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fde17-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fde17-106">提供了为特定应用程序预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="fde17-106">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="fde17-107">将基于模板的任何[同步作业，](synchronization-synchronizationjob.md)默认情况下使用这些设置。</span><span class="sxs-lookup"><span data-stu-id="fde17-107">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="fde17-108">应用程序开发人员指定的模板;任何人都可以检索要查看默认设置，包括[同步架构](synchronization-synchronizationschema.md)的模板。</span><span class="sxs-lookup"><span data-stu-id="fde17-108">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="fde17-109">您可以提供多个模板的应用程序，并指定默认模板。</span><span class="sxs-lookup"><span data-stu-id="fde17-109">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="fde17-110">如果多个模板可供您感兴趣的应用程序，seek 特定于应用程序的指南，以确定哪一个最能满足您的需求。</span><span class="sxs-lookup"><span data-stu-id="fde17-110">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="fde17-111">方法</span><span class="sxs-lookup"><span data-stu-id="fde17-111">Methods</span></span>

| <span data-ttu-id="fde17-112">方法</span><span class="sxs-lookup"><span data-stu-id="fde17-112">Method</span></span>        | <span data-ttu-id="fde17-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="fde17-113">Return Type</span></span>               | <span data-ttu-id="fde17-114">说明</span><span class="sxs-lookup"><span data-stu-id="fde17-114">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="fde17-115">List</span><span class="sxs-lookup"><span data-stu-id="fde17-115">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="fde17-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="fde17-116">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="fde17-117">列表的模板可供应用程序或应用程序实例 （服务主体）。</span><span class="sxs-lookup"><span data-stu-id="fde17-117">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="fde17-118">Get</span><span class="sxs-lookup"><span data-stu-id="fde17-118">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="fde17-119">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="fde17-119">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="fde17-120">读取的属性和**synchronizationTemplate**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="fde17-120">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="fde17-121">属性</span><span class="sxs-lookup"><span data-stu-id="fde17-121">Properties</span></span>

| <span data-ttu-id="fde17-122">属性</span><span class="sxs-lookup"><span data-stu-id="fde17-122">Property</span></span>      | <span data-ttu-id="fde17-123">类型</span><span class="sxs-lookup"><span data-stu-id="fde17-123">Type</span></span>                      | <span data-ttu-id="fde17-124">说明</span><span class="sxs-lookup"><span data-stu-id="fde17-124">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="fde17-125">id</span><span class="sxs-lookup"><span data-stu-id="fde17-125">id</span></span>             |<span data-ttu-id="fde17-126">字符串</span><span class="sxs-lookup"><span data-stu-id="fde17-126">String</span></span>                     |<span data-ttu-id="fde17-127">唯一的模板标识符。</span><span class="sxs-lookup"><span data-stu-id="fde17-127">Unique template identifier.</span></span>|
|<span data-ttu-id="fde17-128">applicationId</span><span class="sxs-lookup"><span data-stu-id="fde17-128">applicationId</span></span>  |<span data-ttu-id="fde17-129">String</span><span class="sxs-lookup"><span data-stu-id="fde17-129">String</span></span>                     |<span data-ttu-id="fde17-130">此模板所属的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="fde17-130">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="fde17-131">default</span><span class="sxs-lookup"><span data-stu-id="fde17-131">default</span></span>        |<span data-ttu-id="fde17-132">布尔</span><span class="sxs-lookup"><span data-stu-id="fde17-132">Boolean</span></span>                    |<span data-ttu-id="fde17-133">`true`如果此模板建议为默认的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fde17-133">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="fde17-134">说明</span><span class="sxs-lookup"><span data-stu-id="fde17-134">description</span></span>    |<span data-ttu-id="fde17-135">字符串</span><span class="sxs-lookup"><span data-stu-id="fde17-135">String</span></span>                     |<span data-ttu-id="fde17-136">模板描述</span><span class="sxs-lookup"><span data-stu-id="fde17-136">Description of the template.</span></span>|
|<span data-ttu-id="fde17-137">可供搜索</span><span class="sxs-lookup"><span data-stu-id="fde17-137">discoverable</span></span>   |<span data-ttu-id="fde17-138">字符串</span><span class="sxs-lookup"><span data-stu-id="fde17-138">String</span></span>                     |<span data-ttu-id="fde17-139">`true`如果此模板应出现在可用应用程序实例 （服务主体） 的模板的集合。</span><span class="sxs-lookup"><span data-stu-id="fde17-139">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="fde17-140">factoryTag</span><span class="sxs-lookup"><span data-stu-id="fde17-140">factoryTag</span></span>     |<span data-ttu-id="fde17-141">字符串</span><span class="sxs-lookup"><span data-stu-id="fde17-141">String</span></span>                     |<span data-ttu-id="fde17-142">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="fde17-142">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="fde17-143">**FactoryTag**告知同步引擎处理在基于此模板的作业时使用的实现。</span><span class="sxs-lookup"><span data-stu-id="fde17-143">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="fde17-144">元数据</span><span class="sxs-lookup"><span data-stu-id="fde17-144">metadata</span></span>       |<span data-ttu-id="fde17-145">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="fde17-145">metadataEntry collection</span></span>   |<span data-ttu-id="fde17-146">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fde17-146">Additional extension properties.</span></span> <span data-ttu-id="fde17-147">除非明确提到，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="fde17-147">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fde17-148">Relationships</span><span class="sxs-lookup"><span data-stu-id="fde17-148">Relationships</span></span>
| <span data-ttu-id="fde17-149">关系</span><span class="sxs-lookup"><span data-stu-id="fde17-149">Relationship</span></span>      | <span data-ttu-id="fde17-150">类型</span><span class="sxs-lookup"><span data-stu-id="fde17-150">Type</span></span>      |<span data-ttu-id="fde17-151">Description</span><span class="sxs-lookup"><span data-stu-id="fde17-151">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="fde17-152">架构</span><span class="sxs-lookup"><span data-stu-id="fde17-152">schema</span></span>             |[<span data-ttu-id="fde17-153">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="fde17-153">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="fde17-154">在基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="fde17-154">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fde17-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fde17-155">JSON representation</span></span>

<span data-ttu-id="fde17-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fde17-156">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
