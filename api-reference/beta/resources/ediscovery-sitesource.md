---
title: siteSource 资源类型
description: 与保管人关联的网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c178565b628728fcf6124ea3058e979f8423ce90
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080475"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="f2897-103">siteSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2897-103">siteSource resource type</span></span>

<span data-ttu-id="f2897-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="f2897-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2897-105">与保管人 关联的网站的 [容器](ediscovery-custodian.md)。</span><span class="sxs-lookup"><span data-stu-id="f2897-105">The container for a site associated with a [custodian](ediscovery-custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f2897-106">方法</span><span class="sxs-lookup"><span data-stu-id="f2897-106">Methods</span></span>

|<span data-ttu-id="f2897-107">方法</span><span class="sxs-lookup"><span data-stu-id="f2897-107">Method</span></span>|<span data-ttu-id="f2897-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2897-108">Return type</span></span>|<span data-ttu-id="f2897-109">说明</span><span class="sxs-lookup"><span data-stu-id="f2897-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2897-110">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="f2897-110">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="f2897-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2897-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="f2897-112">获取 **siteSource 对象** 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="f2897-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="f2897-113">创建 siteSource</span><span class="sxs-lookup"><span data-stu-id="f2897-113">Create siteSource</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="f2897-114">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="f2897-114">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="f2897-115">创建新的 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="f2897-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="f2897-116">获取 siteSource</span><span class="sxs-lookup"><span data-stu-id="f2897-116">Get siteSource</span></span>](../api/ediscovery-sitesource-get.md)|[<span data-ttu-id="f2897-117">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="f2897-117">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="f2897-118">读取 **siteSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2897-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="f2897-119">删除 siteSource</span><span class="sxs-lookup"><span data-stu-id="f2897-119">Delete siteSource</span></span>](../api/ediscovery-sitesource-delete.md)|<span data-ttu-id="f2897-120">无</span><span class="sxs-lookup"><span data-stu-id="f2897-120">None</span></span>|<span data-ttu-id="f2897-121">删除 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="f2897-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f2897-122">属性</span><span class="sxs-lookup"><span data-stu-id="f2897-122">Properties</span></span>

|<span data-ttu-id="f2897-123">属性</span><span class="sxs-lookup"><span data-stu-id="f2897-123">Property</span></span>|<span data-ttu-id="f2897-124">类型</span><span class="sxs-lookup"><span data-stu-id="f2897-124">Type</span></span>|<span data-ttu-id="f2897-125">说明</span><span class="sxs-lookup"><span data-stu-id="f2897-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2897-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="f2897-126">createdBy</span></span>|[<span data-ttu-id="f2897-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="f2897-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="f2897-128">创建 **siteSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="f2897-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="f2897-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2897-129">createdDateTime</span></span>|<span data-ttu-id="f2897-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2897-130">DateTimeOffset</span></span>|<span data-ttu-id="f2897-131">创建 **siteSource 的** 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="f2897-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="f2897-132">displayName</span><span class="sxs-lookup"><span data-stu-id="f2897-132">displayName</span></span>|<span data-ttu-id="f2897-133">String</span><span class="sxs-lookup"><span data-stu-id="f2897-133">String</span></span>|<span data-ttu-id="f2897-134">siteSource 显示名称 **的一部分**。</span><span class="sxs-lookup"><span data-stu-id="f2897-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="f2897-135">这将是网站SharePoint的名称。</span><span class="sxs-lookup"><span data-stu-id="f2897-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="f2897-136">id</span><span class="sxs-lookup"><span data-stu-id="f2897-136">id</span></span>|<span data-ttu-id="f2897-137">String</span><span class="sxs-lookup"><span data-stu-id="f2897-137">String</span></span>| <span data-ttu-id="f2897-138">**siteSource** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="f2897-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="f2897-139">可通过 Get site 随时检索 [网站源](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}</span><span class="sxs-lookup"><span data-stu-id="f2897-139">The site source can be retrieved at any time with [Get site](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2897-140">关系</span><span class="sxs-lookup"><span data-stu-id="f2897-140">Relationships</span></span>

|<span data-ttu-id="f2897-141">关系</span><span class="sxs-lookup"><span data-stu-id="f2897-141">Relationship</span></span>|<span data-ttu-id="f2897-142">类型</span><span class="sxs-lookup"><span data-stu-id="f2897-142">Type</span></span>|<span data-ttu-id="f2897-143">说明</span><span class="sxs-lookup"><span data-stu-id="f2897-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2897-144">网站</span><span class="sxs-lookup"><span data-stu-id="f2897-144">site</span></span>|[<span data-ttu-id="f2897-145">site</span><span class="sxs-lookup"><span data-stu-id="f2897-145">site</span></span>](../resources/site.md)|<span data-ttu-id="f2897-146">与SharePoint网站源 关联的 **网站**。</span><span class="sxs-lookup"><span data-stu-id="f2897-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2897-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2897-147">JSON representation</span></span>

<span data-ttu-id="f2897-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2897-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
