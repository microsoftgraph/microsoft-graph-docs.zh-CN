---
title: siteSource 资源类型
description: 与保管人关联的网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa4b8d0ccbe80ef0f65d27fa8ef648d1ea07b63
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446150"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="4cf5d-103">siteSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cf5d-103">siteSource resource type</span></span>

<span data-ttu-id="4cf5d-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="4cf5d-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cf5d-105">与保管人关联的网站的 [容器](ediscovery-custodian.md)。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-105">The container for a site associated with a [custodian](ediscovery-custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4cf5d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="4cf5d-106">Methods</span></span>

|<span data-ttu-id="4cf5d-107">方法</span><span class="sxs-lookup"><span data-stu-id="4cf5d-107">Method</span></span>|<span data-ttu-id="4cf5d-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4cf5d-108">Return type</span></span>|<span data-ttu-id="4cf5d-109">说明</span><span class="sxs-lookup"><span data-stu-id="4cf5d-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4cf5d-110">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="4cf5d-110">List siteSources</span></span>](../api/ediscovery-custodian-list-sitesources.md)|<span data-ttu-id="4cf5d-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4cf5d-111">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="4cf5d-112">获取 **siteSource 对象** 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="4cf5d-113">创建 siteSource</span><span class="sxs-lookup"><span data-stu-id="4cf5d-113">Create siteSource</span></span>](../api/ediscovery-custodian-post-sitesources.md)|[<span data-ttu-id="4cf5d-114">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="4cf5d-114">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="4cf5d-115">创建新的 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="4cf5d-116">获取 siteSource</span><span class="sxs-lookup"><span data-stu-id="4cf5d-116">Get siteSource</span></span>](../api/ediscovery-sitesource-get.md)|[<span data-ttu-id="4cf5d-117">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="4cf5d-117">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="4cf5d-118">读取 **siteSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="4cf5d-119">删除 siteSource</span><span class="sxs-lookup"><span data-stu-id="4cf5d-119">Delete siteSource</span></span>](../api/ediscovery-sitesource-delete.md)|<span data-ttu-id="4cf5d-120">无</span><span class="sxs-lookup"><span data-stu-id="4cf5d-120">None</span></span>|<span data-ttu-id="4cf5d-121">删除 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4cf5d-122">属性</span><span class="sxs-lookup"><span data-stu-id="4cf5d-122">Properties</span></span>

|<span data-ttu-id="4cf5d-123">属性</span><span class="sxs-lookup"><span data-stu-id="4cf5d-123">Property</span></span>|<span data-ttu-id="4cf5d-124">类型</span><span class="sxs-lookup"><span data-stu-id="4cf5d-124">Type</span></span>|<span data-ttu-id="4cf5d-125">说明</span><span class="sxs-lookup"><span data-stu-id="4cf5d-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf5d-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="4cf5d-126">createdBy</span></span>|[<span data-ttu-id="4cf5d-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="4cf5d-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="4cf5d-128">创建 **siteSource 的用户**。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="4cf5d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4cf5d-129">createdDateTime</span></span>|<span data-ttu-id="4cf5d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4cf5d-130">DateTimeOffset</span></span>|<span data-ttu-id="4cf5d-131">创建 **siteSource 的** 日期和时间。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="4cf5d-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4cf5d-132">displayName</span></span>|<span data-ttu-id="4cf5d-133">String</span><span class="sxs-lookup"><span data-stu-id="4cf5d-133">String</span></span>|<span data-ttu-id="4cf5d-134">siteSource 的 **显示名称。**</span><span class="sxs-lookup"><span data-stu-id="4cf5d-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="4cf5d-135">这将是 SharePoint 网站的名称。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="4cf5d-136">id</span><span class="sxs-lookup"><span data-stu-id="4cf5d-136">id</span></span>|<span data-ttu-id="4cf5d-137">String</span><span class="sxs-lookup"><span data-stu-id="4cf5d-137">String</span></span>| <span data-ttu-id="4cf5d-138">**siteSource** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="4cf5d-139">这不是实际网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-139">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf5d-140">关系</span><span class="sxs-lookup"><span data-stu-id="4cf5d-140">Relationships</span></span>

|<span data-ttu-id="4cf5d-141">关系</span><span class="sxs-lookup"><span data-stu-id="4cf5d-141">Relationship</span></span>|<span data-ttu-id="4cf5d-142">类型</span><span class="sxs-lookup"><span data-stu-id="4cf5d-142">Type</span></span>|<span data-ttu-id="4cf5d-143">说明</span><span class="sxs-lookup"><span data-stu-id="4cf5d-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf5d-144">网站</span><span class="sxs-lookup"><span data-stu-id="4cf5d-144">site</span></span>|[<span data-ttu-id="4cf5d-145">网站</span><span class="sxs-lookup"><span data-stu-id="4cf5d-145">site</span></span>](../resources/site.md)|<span data-ttu-id="4cf5d-146">与 siteSource 关联的 **SharePoint 网站**。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4cf5d-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cf5d-147">JSON representation</span></span>

<span data-ttu-id="4cf5d-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cf5d-148">The following is a JSON representation of the resource.</span></span>
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
