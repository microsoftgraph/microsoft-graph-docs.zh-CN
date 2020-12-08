---
title: siteSource 资源类型
description: 与保管人关联的网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 60b2d8fb3374dd4f97dcff802caf509e66ca6db1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597593"
---
# <a name="sitesource-resource-type"></a><span data-ttu-id="c5e0c-103">siteSource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c5e0c-103">siteSource resource type</span></span>

<span data-ttu-id="c5e0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c5e0c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5e0c-105">与 [保管人](custodian.md)关联的网站的容器。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-105">The container for a site associated with a [custodian](custodian.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c5e0c-106">方法</span><span class="sxs-lookup"><span data-stu-id="c5e0c-106">Methods</span></span>

|<span data-ttu-id="c5e0c-107">方法</span><span class="sxs-lookup"><span data-stu-id="c5e0c-107">Method</span></span>|<span data-ttu-id="c5e0c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="c5e0c-108">Return type</span></span>|<span data-ttu-id="c5e0c-109">Description</span><span class="sxs-lookup"><span data-stu-id="c5e0c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5e0c-110">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="c5e0c-110">List siteSources</span></span>](../api/custodian-list-sitesources.md)|<span data-ttu-id="c5e0c-111">[siteSource](../resources/sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c5e0c-111">[siteSource](../resources/sitesource.md) collection</span></span>|<span data-ttu-id="c5e0c-112">获取 **siteSource** 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-112">Get a list of **siteSource** objects and their properties.</span></span>|
|[<span data-ttu-id="c5e0c-113">创建 siteSource</span><span class="sxs-lookup"><span data-stu-id="c5e0c-113">Create siteSource</span></span>](../api/custodian-post-sitesources.md)|[<span data-ttu-id="c5e0c-114">siteSource</span><span class="sxs-lookup"><span data-stu-id="c5e0c-114">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="c5e0c-115">创建新的 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-115">Create a new **siteSource** object.</span></span>|
|[<span data-ttu-id="c5e0c-116">获取 siteSource</span><span class="sxs-lookup"><span data-stu-id="c5e0c-116">Get siteSource</span></span>](../api/sitesource-get.md)|[<span data-ttu-id="c5e0c-117">siteSource</span><span class="sxs-lookup"><span data-stu-id="c5e0c-117">siteSource</span></span>](../resources/sitesource.md)|<span data-ttu-id="c5e0c-118">读取 **siteSource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-118">Read the properties and relationships of a **siteSource** object.</span></span>|
|[<span data-ttu-id="c5e0c-119">删除 siteSource</span><span class="sxs-lookup"><span data-stu-id="c5e0c-119">Delete siteSource</span></span>](../api/sitesource-delete.md)|<span data-ttu-id="c5e0c-120">无</span><span class="sxs-lookup"><span data-stu-id="c5e0c-120">None</span></span>|<span data-ttu-id="c5e0c-121">删除 **siteSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-121">Delete a **siteSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5e0c-122">属性</span><span class="sxs-lookup"><span data-stu-id="c5e0c-122">Properties</span></span>

|<span data-ttu-id="c5e0c-123">属性</span><span class="sxs-lookup"><span data-stu-id="c5e0c-123">Property</span></span>|<span data-ttu-id="c5e0c-124">类型</span><span class="sxs-lookup"><span data-stu-id="c5e0c-124">Type</span></span>|<span data-ttu-id="c5e0c-125">说明</span><span class="sxs-lookup"><span data-stu-id="c5e0c-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e0c-126">createdBy</span><span class="sxs-lookup"><span data-stu-id="c5e0c-126">createdBy</span></span>|[<span data-ttu-id="c5e0c-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="c5e0c-127">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="c5e0c-128">创建 **siteSource** 的用户。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-128">The user who created the **siteSource**.</span></span>|
|<span data-ttu-id="c5e0c-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c5e0c-129">createdDateTime</span></span>|<span data-ttu-id="c5e0c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5e0c-130">DateTimeOffset</span></span>|<span data-ttu-id="c5e0c-131">**SiteSource** 的创建日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-131">The date and time the **siteSource** was created.</span></span>|
|<span data-ttu-id="c5e0c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="c5e0c-132">displayName</span></span>|<span data-ttu-id="c5e0c-133">String</span><span class="sxs-lookup"><span data-stu-id="c5e0c-133">String</span></span>|<span data-ttu-id="c5e0c-134">**SiteSource** 的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-134">The display name of the **siteSource**.</span></span> <span data-ttu-id="c5e0c-135">这将是 SharePoint 网站的名称。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-135">This will be the name of the SharePoint site.</span></span>|
|<span data-ttu-id="c5e0c-136">id</span><span class="sxs-lookup"><span data-stu-id="c5e0c-136">id</span></span>|<span data-ttu-id="c5e0c-137">String</span><span class="sxs-lookup"><span data-stu-id="c5e0c-137">String</span></span>| <span data-ttu-id="c5e0c-138">**SiteSource** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-138">The ID of the **siteSource**.</span></span> <span data-ttu-id="c5e0c-139">这不是实际网站的 ID。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-139">This is not the ID of the actual site.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5e0c-140">关系</span><span class="sxs-lookup"><span data-stu-id="c5e0c-140">Relationships</span></span>

|<span data-ttu-id="c5e0c-141">关系</span><span class="sxs-lookup"><span data-stu-id="c5e0c-141">Relationship</span></span>|<span data-ttu-id="c5e0c-142">类型</span><span class="sxs-lookup"><span data-stu-id="c5e0c-142">Type</span></span>|<span data-ttu-id="c5e0c-143">Description</span><span class="sxs-lookup"><span data-stu-id="c5e0c-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5e0c-144">网站</span><span class="sxs-lookup"><span data-stu-id="c5e0c-144">site</span></span>|[<span data-ttu-id="c5e0c-145">site</span><span class="sxs-lookup"><span data-stu-id="c5e0c-145">site</span></span>](../resources/site.md)|<span data-ttu-id="c5e0c-146">与 **siteSource** 相关联的 SharePoint 网站。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-146">The SharePoint site associated with the **siteSource**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c5e0c-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c5e0c-147">JSON representation</span></span>

<span data-ttu-id="c5e0c-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c5e0c-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
