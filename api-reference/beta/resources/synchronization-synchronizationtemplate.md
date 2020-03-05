---
title: synchronizationTemplate 资源类型
description: " 任何人都可以检索模板以查看默认设置，包括同步架构。"
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9952b06276efa712068091ecd8b7b5dc5e6769d2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520014"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="d4483-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4483-103">synchronizationTemplate resource type</span></span>

<span data-ttu-id="d4483-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d4483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4483-105">为特定应用程序提供预先配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="d4483-105">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="d4483-106">默认情况下，将对基于该模板的任何[同步作业](synchronization-synchronizationjob.md)使用这些设置。</span><span class="sxs-lookup"><span data-stu-id="d4483-106">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="d4483-107">应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置，包括[同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="d4483-107">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="d4483-108">您可以为应用程序提供多个模板，并指定一个默认模板。</span><span class="sxs-lookup"><span data-stu-id="d4483-108">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="d4483-109">如果有多个模板可用于您感兴趣的应用程序，请查找特定于应用程序的指南，以确定哪一个模板最符合您的需求。</span><span class="sxs-lookup"><span data-stu-id="d4483-109">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="d4483-110">方法</span><span class="sxs-lookup"><span data-stu-id="d4483-110">Methods</span></span>

| <span data-ttu-id="d4483-111">方法</span><span class="sxs-lookup"><span data-stu-id="d4483-111">Method</span></span>        | <span data-ttu-id="d4483-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4483-112">Return Type</span></span>               | <span data-ttu-id="d4483-113">说明</span><span class="sxs-lookup"><span data-stu-id="d4483-113">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="d4483-114">List</span><span class="sxs-lookup"><span data-stu-id="d4483-114">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="d4483-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="d4483-115">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="d4483-116">列出可用于应用程序实例或应用程序实例（服务主体）的模板。</span><span class="sxs-lookup"><span data-stu-id="d4483-116">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="d4483-117">获取</span><span class="sxs-lookup"><span data-stu-id="d4483-117">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="d4483-118">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="d4483-118">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="d4483-119">读取**synchronizationTemplate**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4483-119">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="d4483-120">属性</span><span class="sxs-lookup"><span data-stu-id="d4483-120">Properties</span></span>

| <span data-ttu-id="d4483-121">属性</span><span class="sxs-lookup"><span data-stu-id="d4483-121">Property</span></span>      | <span data-ttu-id="d4483-122">类型</span><span class="sxs-lookup"><span data-stu-id="d4483-122">Type</span></span>                      | <span data-ttu-id="d4483-123">说明</span><span class="sxs-lookup"><span data-stu-id="d4483-123">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="d4483-124">id</span><span class="sxs-lookup"><span data-stu-id="d4483-124">id</span></span>             |<span data-ttu-id="d4483-125">字符串</span><span class="sxs-lookup"><span data-stu-id="d4483-125">String</span></span>                     |<span data-ttu-id="d4483-126">唯一的模板标识符。</span><span class="sxs-lookup"><span data-stu-id="d4483-126">Unique template identifier.</span></span>|
|<span data-ttu-id="d4483-127">applicationId</span><span class="sxs-lookup"><span data-stu-id="d4483-127">applicationId</span></span>  |<span data-ttu-id="d4483-128">String</span><span class="sxs-lookup"><span data-stu-id="d4483-128">String</span></span>                     |<span data-ttu-id="d4483-129">此模板所属应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="d4483-129">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="d4483-130">设置</span><span class="sxs-lookup"><span data-stu-id="d4483-130">default</span></span>        |<span data-ttu-id="d4483-131">布尔</span><span class="sxs-lookup"><span data-stu-id="d4483-131">Boolean</span></span>                    |<span data-ttu-id="d4483-132">`true`如果建议将此模板作为应用程序的默认模板。</span><span class="sxs-lookup"><span data-stu-id="d4483-132">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="d4483-133">说明</span><span class="sxs-lookup"><span data-stu-id="d4483-133">description</span></span>    |<span data-ttu-id="d4483-134">String</span><span class="sxs-lookup"><span data-stu-id="d4483-134">String</span></span>                     |<span data-ttu-id="d4483-135">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="d4483-135">Description of the template.</span></span>|
|<span data-ttu-id="d4483-136">被</span><span class="sxs-lookup"><span data-stu-id="d4483-136">discoverable</span></span>   |<span data-ttu-id="d4483-137">String</span><span class="sxs-lookup"><span data-stu-id="d4483-137">String</span></span>                     |<span data-ttu-id="d4483-138">`true`如果此模板应显示在可用于应用程序实例（服务主体）的模板集合中。</span><span class="sxs-lookup"><span data-stu-id="d4483-138">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="d4483-139">factoryTag</span><span class="sxs-lookup"><span data-stu-id="d4483-139">factoryTag</span></span>     |<span data-ttu-id="d4483-140">String</span><span class="sxs-lookup"><span data-stu-id="d4483-140">String</span></span>                     |<span data-ttu-id="d4483-141">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="d4483-141">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="d4483-142">**FactoryTag**告知同步引擎在处理基于此模板的作业时要使用的实现。</span><span class="sxs-lookup"><span data-stu-id="d4483-142">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="d4483-143">metadata</span><span class="sxs-lookup"><span data-stu-id="d4483-143">metadata</span></span>       |<span data-ttu-id="d4483-144">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="d4483-144">metadataEntry collection</span></span>   |<span data-ttu-id="d4483-145">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="d4483-145">Additional extension properties.</span></span> <span data-ttu-id="d4483-146">除非明确提到，否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="d4483-146">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4483-147">关系</span><span class="sxs-lookup"><span data-stu-id="d4483-147">Relationships</span></span>
| <span data-ttu-id="d4483-148">关系</span><span class="sxs-lookup"><span data-stu-id="d4483-148">Relationship</span></span>      | <span data-ttu-id="d4483-149">类型</span><span class="sxs-lookup"><span data-stu-id="d4483-149">Type</span></span>      |<span data-ttu-id="d4483-150">说明</span><span class="sxs-lookup"><span data-stu-id="d4483-150">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="d4483-151">架构</span><span class="sxs-lookup"><span data-stu-id="d4483-151">schema</span></span>             |[<span data-ttu-id="d4483-152">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="d4483-152">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="d4483-153">基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="d4483-153">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4483-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4483-154">JSON representation</span></span>

<span data-ttu-id="d4483-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4483-155">The following is a JSON representation of the resource.</span></span>

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
