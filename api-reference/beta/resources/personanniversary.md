---
title: personAnniversary 资源类型
description: personAnniversary 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 9c6f979ae1bb0378b22b91494866f724c4fe6628
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997975"
---
# <a name="personanniversary-resource-type"></a><span data-ttu-id="c8842-103">personAnniversary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c8842-103">personAnniversary resource type</span></span>

<span data-ttu-id="c8842-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8842-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8842-105">表示与用户 [配置文件](profile.md)中的人员关联的有意义日期的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c8842-105">Represents the details of meaningful dates associated with a person in a user's [profile](profile.md).</span></span>

<span data-ttu-id="c8842-106">继承自 [itemFacet](itemFacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c8842-107">方法</span><span class="sxs-lookup"><span data-stu-id="c8842-107">Methods</span></span>

|<span data-ttu-id="c8842-108">方法</span><span class="sxs-lookup"><span data-stu-id="c8842-108">Method</span></span>|<span data-ttu-id="c8842-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c8842-109">Return type</span></span>|<span data-ttu-id="c8842-110">说明</span><span class="sxs-lookup"><span data-stu-id="c8842-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c8842-111">列出周年纪念</span><span class="sxs-lookup"><span data-stu-id="c8842-111">List anniversaries</span></span>](../api/profile-list-anniversaries.md)|<span data-ttu-id="c8842-112">[personAnniversary](../resources/personanniversary.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c8842-112">[personAnniversary](../resources/personanniversary.md) collection</span></span>|<span data-ttu-id="c8842-113">从 "周年纪念" 导航属性中获取 personAnniversary 资源。</span><span class="sxs-lookup"><span data-stu-id="c8842-113">Get the personAnniversary resources from the anniversaries navigation property.</span></span>|
|[<span data-ttu-id="c8842-114">创建 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-114">Create personAnniversary</span></span>](../api/profile-post-anniversaries.md)|[<span data-ttu-id="c8842-115">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-115">personAnniversary</span></span>](../resources/personanniversary.md)|<span data-ttu-id="c8842-116">创建新的 personAnniversary 对象。</span><span class="sxs-lookup"><span data-stu-id="c8842-116">Create a new personAnniversary object.</span></span>|
|[<span data-ttu-id="c8842-117">获取 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-117">Get personAnniversary</span></span>](../api/personanniversary-get.md)|[<span data-ttu-id="c8842-118">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-118">personAnniversary</span></span>](../resources/personanniversary.md)|<span data-ttu-id="c8842-119">读取 [personAnniversary](../resources/personanniversary.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c8842-119">Read the properties and relationships of a [personAnniversary](../resources/personanniversary.md) object.</span></span>|
|[<span data-ttu-id="c8842-120">更新 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-120">Update personAnniversary</span></span>](../api/personanniversary-update.md)|[<span data-ttu-id="c8842-121">personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-121">personAnniversary</span></span>](../resources/personanniversary.md)|<span data-ttu-id="c8842-122">更新 [personAnniversary](../resources/personanniversary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8842-122">Update the properties of a [personAnniversary](../resources/personanniversary.md) object.</span></span>|
|[<span data-ttu-id="c8842-123">删除 personAnniversary</span><span class="sxs-lookup"><span data-stu-id="c8842-123">Delete personAnniversary</span></span>](../api/personanniversary-delete.md)|<span data-ttu-id="c8842-124">无</span><span class="sxs-lookup"><span data-stu-id="c8842-124">None</span></span>|<span data-ttu-id="c8842-125">删除一个 [personAnniversary](../resources/personanniversary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c8842-125">Deletes a [personAnniversary](../resources/personanniversary.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c8842-126">属性</span><span class="sxs-lookup"><span data-stu-id="c8842-126">Properties</span></span>

|<span data-ttu-id="c8842-127">属性</span><span class="sxs-lookup"><span data-stu-id="c8842-127">Property</span></span>|<span data-ttu-id="c8842-128">类型</span><span class="sxs-lookup"><span data-stu-id="c8842-128">Type</span></span>|<span data-ttu-id="c8842-129">说明</span><span class="sxs-lookup"><span data-stu-id="c8842-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8842-130">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="c8842-130">allowedAudiences</span></span>|<span data-ttu-id="c8842-131">String</span><span class="sxs-lookup"><span data-stu-id="c8842-131">String</span></span>|<span data-ttu-id="c8842-132">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="c8842-132">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="c8842-133">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-133">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="c8842-134">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c8842-134">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="c8842-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="c8842-135">createdBy</span></span>|[<span data-ttu-id="c8842-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="c8842-136">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="c8842-137">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="c8842-137">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="c8842-138">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-138">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c8842-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c8842-139">createdDateTime</span></span>|<span data-ttu-id="c8842-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8842-140">DateTimeOffset</span></span>|<span data-ttu-id="c8842-141">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="c8842-141">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="c8842-142">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-142">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c8842-143">date</span><span class="sxs-lookup"><span data-stu-id="c8842-143">date</span></span>|<span data-ttu-id="c8842-144">Date</span><span class="sxs-lookup"><span data-stu-id="c8842-144">Date</span></span>|<span data-ttu-id="c8842-145">包含与周年纪念类型相关联的日期。</span><span class="sxs-lookup"><span data-stu-id="c8842-145">Contains the date associated with the anniversary type.</span></span>|
|<span data-ttu-id="c8842-146">id</span><span class="sxs-lookup"><span data-stu-id="c8842-146">id</span></span>|<span data-ttu-id="c8842-147">String</span><span class="sxs-lookup"><span data-stu-id="c8842-147">String</span></span>|<span data-ttu-id="c8842-148">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="c8842-148">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="c8842-149">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="c8842-149">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="c8842-150">推导</span><span class="sxs-lookup"><span data-stu-id="c8842-150">inference</span></span>|[<span data-ttu-id="c8842-151">inferenceData</span><span class="sxs-lookup"><span data-stu-id="c8842-151">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="c8842-152">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="c8842-152">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="c8842-153">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-153">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c8842-154">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c8842-154">lastModifiedBy</span></span>|[<span data-ttu-id="c8842-155">identitySet</span><span class="sxs-lookup"><span data-stu-id="c8842-155">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="c8842-156">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="c8842-156">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="c8842-157">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-157">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c8842-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c8842-158">lastModifiedDateTime</span></span>|<span data-ttu-id="c8842-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8842-159">DateTimeOffset</span></span>|<span data-ttu-id="c8842-160">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="c8842-160">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="c8842-161">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-161">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c8842-162">source</span><span class="sxs-lookup"><span data-stu-id="c8842-162">source</span></span>|[<span data-ttu-id="c8842-163">personDataSource</span><span class="sxs-lookup"><span data-stu-id="c8842-163">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="c8842-164">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="c8842-164">Where the values originated if synced from another service.</span></span> <span data-ttu-id="c8842-165">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="c8842-165">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="c8842-166">type</span><span class="sxs-lookup"><span data-stu-id="c8842-166">type</span></span>|<span data-ttu-id="c8842-167">anniversaryType</span><span class="sxs-lookup"><span data-stu-id="c8842-167">anniversaryType</span></span>|<span data-ttu-id="c8842-168">日期所代表的周年纪念的类型。</span><span class="sxs-lookup"><span data-stu-id="c8842-168">The type of anniversary the date represents.</span></span> <span data-ttu-id="c8842-169">可取值为：`birthday`、`wedding`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="c8842-169">Possible values are: `birthday`, `wedding`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8842-170">关系</span><span class="sxs-lookup"><span data-stu-id="c8842-170">Relationships</span></span>
<span data-ttu-id="c8842-171">无。</span><span class="sxs-lookup"><span data-stu-id="c8842-171">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8842-172">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c8842-172">JSON representation</span></span>
<span data-ttu-id="c8842-173">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8842-173">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personAnniversary",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personAnniversary",
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
  "type": "String",
  "date": "Date"
}
```


