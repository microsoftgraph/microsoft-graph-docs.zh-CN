---
title: itemAddress 资源类型
description: itemAddress 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ca6848b6b5ac60d419e56914a59e2470d5970ed9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075635"
---
# <a name="itemaddress-resource-type"></a><span data-ttu-id="a5c79-103">itemAddress 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5c79-103">itemAddress resource type</span></span>

<span data-ttu-id="a5c79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5c79-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a5c79-105">表示物理地址以及找到地址的位置的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5c79-105">Represents a physical address and details of the location where the address is found.</span></span>

<span data-ttu-id="a5c79-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a5c79-107">方法</span><span class="sxs-lookup"><span data-stu-id="a5c79-107">Methods</span></span>
|<span data-ttu-id="a5c79-108">方法</span><span class="sxs-lookup"><span data-stu-id="a5c79-108">Method</span></span>|<span data-ttu-id="a5c79-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a5c79-109">Return type</span></span>|<span data-ttu-id="a5c79-110">说明</span><span class="sxs-lookup"><span data-stu-id="a5c79-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a5c79-111">列表地址</span><span class="sxs-lookup"><span data-stu-id="a5c79-111">List addresses</span></span>](../api/profile-list-addresses.md)|<span data-ttu-id="a5c79-112">[itemAddress](../resources/itemaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5c79-112">[itemAddress](../resources/itemaddress.md) collection</span></span>|<span data-ttu-id="a5c79-113">从 "地址" 导航属性中获取 itemAddress 资源。</span><span class="sxs-lookup"><span data-stu-id="a5c79-113">Get the itemAddress resources from the addresses navigation property.</span></span>|
|[<span data-ttu-id="a5c79-114">创建 itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-114">Create itemAddress</span></span>](../api/profile-post-addresses.md)|[<span data-ttu-id="a5c79-115">itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-115">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="a5c79-116">创建新的 itemAddress 对象。</span><span class="sxs-lookup"><span data-stu-id="a5c79-116">Create a new itemAddress object.</span></span>|
|[<span data-ttu-id="a5c79-117">获取 itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-117">Get itemAddress</span></span>](../api/itemaddress-get.md)|[<span data-ttu-id="a5c79-118">itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-118">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="a5c79-119">读取 [itemAddress](../resources/itemaddress.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a5c79-119">Read the properties and relationships of an [itemAddress](../resources/itemaddress.md) object.</span></span>|
|[<span data-ttu-id="a5c79-120">更新 itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-120">Update itemAddress</span></span>](../api/itemaddress-update.md)|[<span data-ttu-id="a5c79-121">itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-121">itemAddress</span></span>](../resources/itemaddress.md)|<span data-ttu-id="a5c79-122">更新 [itemAddress](../resources/itemaddress.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a5c79-122">Update the properties of an [itemAddress](../resources/itemaddress.md) object.</span></span>|
|[<span data-ttu-id="a5c79-123">删除 itemAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-123">Delete itemAddress</span></span>](../api/itemaddress-delete.md)|<span data-ttu-id="a5c79-124">无</span><span class="sxs-lookup"><span data-stu-id="a5c79-124">None</span></span>|<span data-ttu-id="a5c79-125">删除一个 [itemAddress](../resources/itemaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a5c79-125">Deletes an [itemAddress](../resources/itemaddress.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a5c79-126">属性</span><span class="sxs-lookup"><span data-stu-id="a5c79-126">Properties</span></span>
|<span data-ttu-id="a5c79-127">属性</span><span class="sxs-lookup"><span data-stu-id="a5c79-127">Property</span></span>|<span data-ttu-id="a5c79-128">类型</span><span class="sxs-lookup"><span data-stu-id="a5c79-128">Type</span></span>|<span data-ttu-id="a5c79-129">说明</span><span class="sxs-lookup"><span data-stu-id="a5c79-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5c79-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="a5c79-130">allowedAudiences</span></span>|<span data-ttu-id="a5c79-131">String</span><span class="sxs-lookup"><span data-stu-id="a5c79-131">String</span></span>|<span data-ttu-id="a5c79-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="a5c79-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="a5c79-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="a5c79-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="a5c79-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a5c79-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="a5c79-135">createdBy</span></span>|[<span data-ttu-id="a5c79-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="a5c79-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a5c79-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a5c79-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="a5c79-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a5c79-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c79-139">createdDateTime</span></span>|<span data-ttu-id="a5c79-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c79-140">DateTimeOffset</span></span>|<span data-ttu-id="a5c79-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a5c79-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="a5c79-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a5c79-143">介绍</span><span class="sxs-lookup"><span data-stu-id="a5c79-143">detail</span></span>|[<span data-ttu-id="a5c79-144">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a5c79-144">physicalAddress</span></span>](../resources/physicaladdress.md)|<span data-ttu-id="a5c79-145">地址本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5c79-145">Details about the address itself.</span></span>|
|<span data-ttu-id="a5c79-146">displayName</span><span class="sxs-lookup"><span data-stu-id="a5c79-146">displayName</span></span>|<span data-ttu-id="a5c79-147">String</span><span class="sxs-lookup"><span data-stu-id="a5c79-147">String</span></span>|<span data-ttu-id="a5c79-148">用户已分配到此地址的友好名称。</span><span class="sxs-lookup"><span data-stu-id="a5c79-148">Friendly name the user has assigned to this address.</span></span> |
|<span data-ttu-id="a5c79-149">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a5c79-149">geoCoordinates</span></span>|[<span data-ttu-id="a5c79-150">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="a5c79-150">geoCoordinates</span></span>](../resources/geocoordinates.md)|<span data-ttu-id="a5c79-151">地址的 geocoordinates。</span><span class="sxs-lookup"><span data-stu-id="a5c79-151">The geocoordinates of the address.</span></span>|
|<span data-ttu-id="a5c79-152">id</span><span class="sxs-lookup"><span data-stu-id="a5c79-152">id</span></span>|<span data-ttu-id="a5c79-153">String</span><span class="sxs-lookup"><span data-stu-id="a5c79-153">String</span></span>|<span data-ttu-id="a5c79-154">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="a5c79-154">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="a5c79-155">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="a5c79-155">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="a5c79-156">推导</span><span class="sxs-lookup"><span data-stu-id="a5c79-156">inference</span></span>|[<span data-ttu-id="a5c79-157">inferenceData</span><span class="sxs-lookup"><span data-stu-id="a5c79-157">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="a5c79-158">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="a5c79-158">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="a5c79-159">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-159">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a5c79-160">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="a5c79-160">lastModifiedBy</span></span>|[<span data-ttu-id="a5c79-161">identitySet</span><span class="sxs-lookup"><span data-stu-id="a5c79-161">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a5c79-162">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a5c79-162">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="a5c79-163">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-163">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a5c79-164">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5c79-164">lastModifiedDateTime</span></span>|<span data-ttu-id="a5c79-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5c79-165">DateTimeOffset</span></span>|<span data-ttu-id="a5c79-166">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a5c79-166">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="a5c79-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="a5c79-168">source</span><span class="sxs-lookup"><span data-stu-id="a5c79-168">source</span></span>|[<span data-ttu-id="a5c79-169">personDataSource</span><span class="sxs-lookup"><span data-stu-id="a5c79-169">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="a5c79-170">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="a5c79-170">Where the values originated if synced from another service.</span></span> <span data-ttu-id="a5c79-171">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="a5c79-171">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5c79-172">关系</span><span class="sxs-lookup"><span data-stu-id="a5c79-172">Relationships</span></span>
<span data-ttu-id="a5c79-173">无。</span><span class="sxs-lookup"><span data-stu-id="a5c79-173">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a5c79-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5c79-174">JSON representation</span></span>
<span data-ttu-id="a5c79-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5c79-175">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAddress",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAddress",
  "id": "String (identifier)",
  "allowedAudiences": "String",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "String",
  "detail": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.geoCoordinates"
  }
}
```


