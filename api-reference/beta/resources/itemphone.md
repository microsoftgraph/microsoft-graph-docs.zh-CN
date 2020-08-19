---
title: itemPhone 资源类型
description: itemPhone 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0c36ea4d861738316a3ce6593c12a79a59d97c68
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809402"
---
# <a name="itemphone-resource-type"></a><span data-ttu-id="47037-103">itemPhone 资源类型</span><span class="sxs-lookup"><span data-stu-id="47037-103">itemPhone resource type</span></span>

<span data-ttu-id="47037-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47037-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="47037-105">表示有关与各种服务中的用户关联的电话号码的详细信息。</span><span class="sxs-lookup"><span data-stu-id="47037-105">Represents detailed information about phone numbers associated with a user in various services.</span></span>

<span data-ttu-id="47037-106">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-106">Inherits from [itemFacet](../resources/itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="47037-107">方法</span><span class="sxs-lookup"><span data-stu-id="47037-107">Methods</span></span>

|<span data-ttu-id="47037-108">方法</span><span class="sxs-lookup"><span data-stu-id="47037-108">Method</span></span>|<span data-ttu-id="47037-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="47037-109">Return type</span></span>|<span data-ttu-id="47037-110">说明</span><span class="sxs-lookup"><span data-stu-id="47037-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="47037-111">列出电话</span><span class="sxs-lookup"><span data-stu-id="47037-111">List phones</span></span>](../api/profile-list-phones.md)|<span data-ttu-id="47037-112">[itemPhone](../resources/itemphone.md) 集合</span><span class="sxs-lookup"><span data-stu-id="47037-112">[itemPhone](../resources/itemphone.md) collection</span></span>|<span data-ttu-id="47037-113">从 "电话" 导航属性中获取 itemPhone 资源。</span><span class="sxs-lookup"><span data-stu-id="47037-113">Get the itemPhone resources from the phones navigation property.</span></span>|
|[<span data-ttu-id="47037-114">创建 itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-114">Create itemPhone</span></span>](../api/profile-post-phones.md)|[<span data-ttu-id="47037-115">itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-115">itemPhone</span></span>](../resources/itemphone.md)|<span data-ttu-id="47037-116">创建新的 itemPhone 对象。</span><span class="sxs-lookup"><span data-stu-id="47037-116">Create a new itemPhone object.</span></span>|
|[<span data-ttu-id="47037-117">获取 itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-117">Get itemPhone</span></span>](../api/itemphone-get.md)|[<span data-ttu-id="47037-118">itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-118">itemPhone</span></span>](../resources/itemphone.md)|<span data-ttu-id="47037-119">读取 [itemPhone](../resources/itemphone.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="47037-119">Read the properties and relationships of an [itemPhone](../resources/itemphone.md) object.</span></span>|
|[<span data-ttu-id="47037-120">更新 itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-120">Update itemPhone</span></span>](../api/itemphone-update.md)|[<span data-ttu-id="47037-121">itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-121">itemPhone</span></span>](../resources/itemphone.md)|<span data-ttu-id="47037-122">更新 [itemPhone](../resources/itemphone.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="47037-122">Update the properties of an [itemPhone](../resources/itemphone.md) object.</span></span>|
|[<span data-ttu-id="47037-123">删除 itemPhone</span><span class="sxs-lookup"><span data-stu-id="47037-123">Delete itemPhone</span></span>](../api/itemphone-delete.md)|<span data-ttu-id="47037-124">无</span><span class="sxs-lookup"><span data-stu-id="47037-124">None</span></span>|<span data-ttu-id="47037-125">删除一个 [itemPhone](../resources/itemphone.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="47037-125">Deletes an [itemPhone](../resources/itemphone.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="47037-126">属性</span><span class="sxs-lookup"><span data-stu-id="47037-126">Properties</span></span>

|<span data-ttu-id="47037-127">属性</span><span class="sxs-lookup"><span data-stu-id="47037-127">Property</span></span>|<span data-ttu-id="47037-128">类型</span><span class="sxs-lookup"><span data-stu-id="47037-128">Type</span></span>|<span data-ttu-id="47037-129">说明</span><span class="sxs-lookup"><span data-stu-id="47037-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47037-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="47037-130">allowedAudiences</span></span>|<span data-ttu-id="47037-131">String</span><span class="sxs-lookup"><span data-stu-id="47037-131">String</span></span>|<span data-ttu-id="47037-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="47037-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="47037-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="47037-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="47037-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="47037-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="47037-135">createdBy</span></span>|[<span data-ttu-id="47037-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="47037-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="47037-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="47037-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="47037-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="47037-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="47037-139">createdDateTime</span></span>|<span data-ttu-id="47037-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47037-140">DateTimeOffset</span></span>|<span data-ttu-id="47037-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="47037-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="47037-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="47037-143">displayName</span><span class="sxs-lookup"><span data-stu-id="47037-143">displayName</span></span>|<span data-ttu-id="47037-144">String</span><span class="sxs-lookup"><span data-stu-id="47037-144">String</span></span>|<span data-ttu-id="47037-145">友好名称用户已分配了此电话号码。</span><span class="sxs-lookup"><span data-stu-id="47037-145">Friendly name the user has assigned this phone number.</span></span> |
|<span data-ttu-id="47037-146">id</span><span class="sxs-lookup"><span data-stu-id="47037-146">id</span></span>|<span data-ttu-id="47037-147">String</span><span class="sxs-lookup"><span data-stu-id="47037-147">String</span></span>|<span data-ttu-id="47037-148">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="47037-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="47037-149">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="47037-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="47037-150">推导</span><span class="sxs-lookup"><span data-stu-id="47037-150">inference</span></span>|[<span data-ttu-id="47037-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="47037-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="47037-152">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="47037-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="47037-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="47037-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="47037-154">lastModifiedBy</span></span>|[<span data-ttu-id="47037-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="47037-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="47037-156">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="47037-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="47037-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="47037-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="47037-158">lastModifiedDateTime</span></span>|<span data-ttu-id="47037-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="47037-159">DateTimeOffset</span></span>|<span data-ttu-id="47037-160">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="47037-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="47037-161">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="47037-162">数字</span><span class="sxs-lookup"><span data-stu-id="47037-162">number</span></span>|<span data-ttu-id="47037-163">String</span><span class="sxs-lookup"><span data-stu-id="47037-163">String</span></span>|<span data-ttu-id="47037-164">用户提供的电话号码。</span><span class="sxs-lookup"><span data-stu-id="47037-164">Phone number provided by the user.</span></span>|
|<span data-ttu-id="47037-165">source</span><span class="sxs-lookup"><span data-stu-id="47037-165">source</span></span>|[<span data-ttu-id="47037-166">personDataSource</span><span class="sxs-lookup"><span data-stu-id="47037-166">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="47037-167">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="47037-167">Where the values originated if synced from another service.</span></span> <span data-ttu-id="47037-168">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="47037-168">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="47037-169">type</span><span class="sxs-lookup"><span data-stu-id="47037-169">type</span></span>|<span data-ttu-id="47037-170">phoneType</span><span class="sxs-lookup"><span data-stu-id="47037-170">phoneType</span></span>|<span data-ttu-id="47037-171">对象中的电话号码的类型。</span><span class="sxs-lookup"><span data-stu-id="47037-171">The type of phone number within the object.</span></span> <span data-ttu-id="47037-172">可取值为：`home`、`business`、`mobile`、`other`、`assistant`、`homeFax`、`businessFax`、`otherFax`、`pager`、`radio`。</span><span class="sxs-lookup"><span data-stu-id="47037-172">Possible values are: `home`, `business`, `mobile`, `other`, `assistant`, `homeFax`, `businessFax`, `otherFax`, `pager`, `radio`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47037-173">关系</span><span class="sxs-lookup"><span data-stu-id="47037-173">Relationships</span></span>

<span data-ttu-id="47037-174">无。</span><span class="sxs-lookup"><span data-stu-id="47037-174">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="47037-175">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="47037-175">JSON representation</span></span>

<span data-ttu-id="47037-176">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47037-176">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemPhone",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.itemPhone",
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
  "type": "String",
  "number": "String"
}
```
