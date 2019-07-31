---
title: synchronizationTemplate 资源类型
description: " 任何人都可以检索模板以查看默认设置, 包括同步架构。"
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a9176c092d62b4ee43d15d29884a3882fd3c627e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964597"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="4d7dd-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="4d7dd-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d7dd-104">为特定应用程序提供预先配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="4d7dd-105">默认情况下, 将对基于该模板的任何[同步作业](synchronization-synchronizationjob.md)使用这些设置。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="4d7dd-106">应用程序开发人员指定模板;任何人都可以检索模板以查看默认设置, 包括[同步架构](synchronization-synchronizationschema.md)。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="4d7dd-107">您可以为应用程序提供多个模板, 并指定一个默认模板。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="4d7dd-108">如果有多个模板可用于您感兴趣的应用程序, 请查找特定于应用程序的指南, 以确定哪一个模板最符合您的需求。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="4d7dd-109">方法</span><span class="sxs-lookup"><span data-stu-id="4d7dd-109">Methods</span></span>

| <span data-ttu-id="4d7dd-110">方法</span><span class="sxs-lookup"><span data-stu-id="4d7dd-110">Method</span></span>        | <span data-ttu-id="4d7dd-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="4d7dd-111">Return Type</span></span>               | <span data-ttu-id="4d7dd-112">说明</span><span class="sxs-lookup"><span data-stu-id="4d7dd-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="4d7dd-113">List</span><span class="sxs-lookup"><span data-stu-id="4d7dd-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="4d7dd-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="4d7dd-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="4d7dd-115">列出可用于应用程序实例或应用程序实例 (服务主体) 的模板。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="4d7dd-116">获取</span><span class="sxs-lookup"><span data-stu-id="4d7dd-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="4d7dd-117">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="4d7dd-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="4d7dd-118">读取**synchronizationTemplate**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="4d7dd-119">属性</span><span class="sxs-lookup"><span data-stu-id="4d7dd-119">Properties</span></span>

| <span data-ttu-id="4d7dd-120">属性</span><span class="sxs-lookup"><span data-stu-id="4d7dd-120">Property</span></span>      | <span data-ttu-id="4d7dd-121">类型</span><span class="sxs-lookup"><span data-stu-id="4d7dd-121">Type</span></span>                      | <span data-ttu-id="4d7dd-122">说明</span><span class="sxs-lookup"><span data-stu-id="4d7dd-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="4d7dd-123">id</span><span class="sxs-lookup"><span data-stu-id="4d7dd-123">id</span></span>             |<span data-ttu-id="4d7dd-124">字符串</span><span class="sxs-lookup"><span data-stu-id="4d7dd-124">String</span></span>                     |<span data-ttu-id="4d7dd-125">唯一的模板标识符。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-125">Unique template identifier.</span></span>|
|<span data-ttu-id="4d7dd-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="4d7dd-126">applicationId</span></span>  |<span data-ttu-id="4d7dd-127">String</span><span class="sxs-lookup"><span data-stu-id="4d7dd-127">String</span></span>                     |<span data-ttu-id="4d7dd-128">此模板所属应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="4d7dd-129">设置</span><span class="sxs-lookup"><span data-stu-id="4d7dd-129">default</span></span>        |<span data-ttu-id="4d7dd-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="4d7dd-130">Boolean</span></span>                    |<span data-ttu-id="4d7dd-131">`true`如果建议将此模板作为应用程序的默认模板。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="4d7dd-132">说明</span><span class="sxs-lookup"><span data-stu-id="4d7dd-132">description</span></span>    |<span data-ttu-id="4d7dd-133">String</span><span class="sxs-lookup"><span data-stu-id="4d7dd-133">String</span></span>                     |<span data-ttu-id="4d7dd-134">模板的说明。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-134">Description of the template.</span></span>|
|<span data-ttu-id="4d7dd-135">被</span><span class="sxs-lookup"><span data-stu-id="4d7dd-135">discoverable</span></span>   |<span data-ttu-id="4d7dd-136">String</span><span class="sxs-lookup"><span data-stu-id="4d7dd-136">String</span></span>                     |<span data-ttu-id="4d7dd-137">`true`如果此模板应显示在可用于应用程序实例 (服务主体) 的模板集合中。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="4d7dd-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="4d7dd-138">factoryTag</span></span>     |<span data-ttu-id="4d7dd-139">String</span><span class="sxs-lookup"><span data-stu-id="4d7dd-139">String</span></span>                     |<span data-ttu-id="4d7dd-140">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="4d7dd-141">**FactoryTag**告知同步引擎在处理基于此模板的作业时要使用的实现。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="4d7dd-142">metadata</span><span class="sxs-lookup"><span data-stu-id="4d7dd-142">metadata</span></span>       |<span data-ttu-id="4d7dd-143">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="4d7dd-143">metadataEntry collection</span></span>   |<span data-ttu-id="4d7dd-144">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-144">Additional extension properties.</span></span> <span data-ttu-id="4d7dd-145">除非明确提到, 否则不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4d7dd-146">关系</span><span class="sxs-lookup"><span data-stu-id="4d7dd-146">Relationships</span></span>
| <span data-ttu-id="4d7dd-147">关系</span><span class="sxs-lookup"><span data-stu-id="4d7dd-147">Relationship</span></span>      | <span data-ttu-id="4d7dd-148">类型</span><span class="sxs-lookup"><span data-stu-id="4d7dd-148">Type</span></span>      |<span data-ttu-id="4d7dd-149">说明</span><span class="sxs-lookup"><span data-stu-id="4d7dd-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="4d7dd-150">架构</span><span class="sxs-lookup"><span data-stu-id="4d7dd-150">schema</span></span>             |[<span data-ttu-id="4d7dd-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="4d7dd-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="4d7dd-152">基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d7dd-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4d7dd-153">JSON representation</span></span>

<span data-ttu-id="4d7dd-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4d7dd-154">The following is a JSON representation of the resource.</span></span>

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
