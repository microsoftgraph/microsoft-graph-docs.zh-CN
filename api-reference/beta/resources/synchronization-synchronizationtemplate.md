---
title: synchronizationTemplate 资源类型
description: " 任何人都可以检索要查看默认设置，包括同步架构的模板。"
localization_priority: Normal
ms.openlocfilehash: 75df13d55cfb58aafe8a751279e103424aa29367
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516551"
---
# <a name="synchronizationtemplate-resource-type"></a><span data-ttu-id="adb0e-103">synchronizationTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="adb0e-103">synchronizationTemplate resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adb0e-104">提供了为特定应用程序预配置的同步设置。</span><span class="sxs-lookup"><span data-stu-id="adb0e-104">Provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="adb0e-105">将基于模板的任何[同步作业，](synchronization-synchronizationjob.md)默认情况下使用这些设置。</span><span class="sxs-lookup"><span data-stu-id="adb0e-105">These settings will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="adb0e-106">应用程序开发人员指定的模板;任何人都可以检索要查看默认设置，包括[同步架构](synchronization-synchronizationschema.md)的模板。</span><span class="sxs-lookup"><span data-stu-id="adb0e-106">The application developer specifies the template; anyone can retrieve the template to see the default settings, including the [synchronization schema](synchronization-synchronizationschema.md).</span></span>

<span data-ttu-id="adb0e-107">您可以提供多个模板的应用程序，并指定默认模板。</span><span class="sxs-lookup"><span data-stu-id="adb0e-107">You can provide multiple templates for an application, and designate a default template.</span></span> <span data-ttu-id="adb0e-108">如果多个模板可供您感兴趣的应用程序，seek 特定于应用程序的指南，以确定哪一个最能满足您的需求。</span><span class="sxs-lookup"><span data-stu-id="adb0e-108">If multiple templates are available for the application you're interested in, seek application-specific guidance to determine which one best meets your needs.</span></span>

## <a name="methods"></a><span data-ttu-id="adb0e-109">方法</span><span class="sxs-lookup"><span data-stu-id="adb0e-109">Methods</span></span>

| <span data-ttu-id="adb0e-110">方法</span><span class="sxs-lookup"><span data-stu-id="adb0e-110">Method</span></span>        | <span data-ttu-id="adb0e-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="adb0e-111">Return Type</span></span>               | <span data-ttu-id="adb0e-112">说明</span><span class="sxs-lookup"><span data-stu-id="adb0e-112">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|[<span data-ttu-id="adb0e-113">List</span><span class="sxs-lookup"><span data-stu-id="adb0e-113">List</span></span>](../api/synchronization-synchronizationtemplate-list.md)    |<span data-ttu-id="adb0e-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md)集合</span><span class="sxs-lookup"><span data-stu-id="adb0e-114">[synchronizationTemplate](synchronization-synchronizationtemplate.md) collection</span></span>  |<span data-ttu-id="adb0e-115">列表的模板可供应用程序或应用程序实例 （服务主体）。</span><span class="sxs-lookup"><span data-stu-id="adb0e-115">List the templates that are available for an application or application instance (service principal).</span></span>|
|[<span data-ttu-id="adb0e-116">Get</span><span class="sxs-lookup"><span data-stu-id="adb0e-116">Get</span></span>](../api/synchronization-synchronizationtemplate-get.md)      |[<span data-ttu-id="adb0e-117">synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="adb0e-117">synchronizationTemplate</span></span>](synchronization-synchronizationtemplate.md)   |<span data-ttu-id="adb0e-118">读取的属性和**synchronizationTemplate**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="adb0e-118">Read the properties and relationships of the **synchronizationTemplate** object.</span></span>|
<!-- 
|[Create](../api/synchronization-synchronizationtemplate-post.md) |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Create a new template for an application.|
|[Update](../api/synchronization-synchronizationtemplate-put.md)   |[synchronizationTemplate](synchronization-synchronizationtemplate.md)   |Update the template.| 
-->

## <a name="properties"></a><span data-ttu-id="adb0e-119">属性</span><span class="sxs-lookup"><span data-stu-id="adb0e-119">Properties</span></span>

| <span data-ttu-id="adb0e-120">属性</span><span class="sxs-lookup"><span data-stu-id="adb0e-120">Property</span></span>      | <span data-ttu-id="adb0e-121">类型</span><span class="sxs-lookup"><span data-stu-id="adb0e-121">Type</span></span>                      | <span data-ttu-id="adb0e-122">说明</span><span class="sxs-lookup"><span data-stu-id="adb0e-122">Description</span></span>                  |
|:--------------|:--------------------------|:-----------------------------|
|<span data-ttu-id="adb0e-123">id</span><span class="sxs-lookup"><span data-stu-id="adb0e-123">id</span></span>             |<span data-ttu-id="adb0e-124">String</span><span class="sxs-lookup"><span data-stu-id="adb0e-124">String</span></span>                     |<span data-ttu-id="adb0e-125">唯一的模板标识符。</span><span class="sxs-lookup"><span data-stu-id="adb0e-125">Unique template identifier.</span></span>|
|<span data-ttu-id="adb0e-126">applicationId</span><span class="sxs-lookup"><span data-stu-id="adb0e-126">applicationId</span></span>  |<span data-ttu-id="adb0e-127">String</span><span class="sxs-lookup"><span data-stu-id="adb0e-127">String</span></span>                     |<span data-ttu-id="adb0e-128">此模板所属的应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="adb0e-128">Identifier of the application this template belongs to.</span></span>|
|<span data-ttu-id="adb0e-129">default</span><span class="sxs-lookup"><span data-stu-id="adb0e-129">default</span></span>        |<span data-ttu-id="adb0e-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="adb0e-130">Boolean</span></span>                    |<span data-ttu-id="adb0e-131">`true`如果此模板建议为默认的应用程序。</span><span class="sxs-lookup"><span data-stu-id="adb0e-131">`true` if this template is recommended to be the default for the application.</span></span>|
|<span data-ttu-id="adb0e-132">说明</span><span class="sxs-lookup"><span data-stu-id="adb0e-132">description</span></span>    |<span data-ttu-id="adb0e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="adb0e-133">String</span></span>                     |<span data-ttu-id="adb0e-134">模板描述</span><span class="sxs-lookup"><span data-stu-id="adb0e-134">Description of the template.</span></span>|
|<span data-ttu-id="adb0e-135">可供搜索</span><span class="sxs-lookup"><span data-stu-id="adb0e-135">discoverable</span></span>   |<span data-ttu-id="adb0e-136">String</span><span class="sxs-lookup"><span data-stu-id="adb0e-136">String</span></span>                     |<span data-ttu-id="adb0e-137">`true`如果此模板应出现在可用应用程序实例 （服务主体） 的模板的集合。</span><span class="sxs-lookup"><span data-stu-id="adb0e-137">`true` if this template should appear in the collection of templates available for the application instance (service principal).</span></span>|
|<span data-ttu-id="adb0e-138">factoryTag</span><span class="sxs-lookup"><span data-stu-id="adb0e-138">factoryTag</span></span>     |<span data-ttu-id="adb0e-139">String</span><span class="sxs-lookup"><span data-stu-id="adb0e-139">String</span></span>                     |<span data-ttu-id="adb0e-140">同步引擎支持的已知工厂标记之一。</span><span class="sxs-lookup"><span data-stu-id="adb0e-140">One of the well-known factory tags supported by the synchronization engine.</span></span> <span data-ttu-id="adb0e-141">**FactoryTag**告知同步引擎处理在基于此模板的作业时使用的实现。</span><span class="sxs-lookup"><span data-stu-id="adb0e-141">The **factoryTag** tells the synchronization engine which implementation to use when processing jobs based on this template.</span></span>|
|<span data-ttu-id="adb0e-142">元数据</span><span class="sxs-lookup"><span data-stu-id="adb0e-142">metadata</span></span>       |<span data-ttu-id="adb0e-143">metadataEntry 集合</span><span class="sxs-lookup"><span data-stu-id="adb0e-143">metadataEntry collection</span></span>   |<span data-ttu-id="adb0e-144">其他扩展属性。</span><span class="sxs-lookup"><span data-stu-id="adb0e-144">Additional extension properties.</span></span> <span data-ttu-id="adb0e-145">除非明确提到，不应更改元数据值。</span><span class="sxs-lookup"><span data-stu-id="adb0e-145">Unless mentioned explicitly, metadata values should not be changed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="adb0e-146">关系</span><span class="sxs-lookup"><span data-stu-id="adb0e-146">Relationships</span></span>
| <span data-ttu-id="adb0e-147">关系</span><span class="sxs-lookup"><span data-stu-id="adb0e-147">Relationship</span></span>      | <span data-ttu-id="adb0e-148">类型</span><span class="sxs-lookup"><span data-stu-id="adb0e-148">Type</span></span>      |<span data-ttu-id="adb0e-149">说明</span><span class="sxs-lookup"><span data-stu-id="adb0e-149">Description</span></span>|
|:------------------|:----------|:----------|
|<span data-ttu-id="adb0e-150">架构</span><span class="sxs-lookup"><span data-stu-id="adb0e-150">schema</span></span>             |[<span data-ttu-id="adb0e-151">synchronizationSchema</span><span class="sxs-lookup"><span data-stu-id="adb0e-151">synchronizationSchema</span></span>](synchronization-synchronizationschema.md)     |<span data-ttu-id="adb0e-152">在基于此模板的作业的默认同步架构。</span><span class="sxs-lookup"><span data-stu-id="adb0e-152">Default synchronization schema for the jobs based on this template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="adb0e-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="adb0e-153">JSON representation</span></span>

<span data-ttu-id="adb0e-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adb0e-154">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/synchronization-synchronizationtemplate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
