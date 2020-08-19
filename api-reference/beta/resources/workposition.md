---
title: workPosition 资源类型
description: workPosition 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e9a13bc36b2ed1eb42b4155e86d69826b0c22d9d
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810354"
---
# <a name="workposition-resource-type"></a><span data-ttu-id="6fb73-103">workPosition 资源类型</span><span class="sxs-lookup"><span data-stu-id="6fb73-103">workPosition resource type</span></span>

<span data-ttu-id="6fb73-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fb73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6fb73-105">表示有关与用户 [配置文件](profile.md)相关联的工作职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fb73-105">Represents detailed information about work positions associated with a user's [profile](profile.md).</span></span>

<span data-ttu-id="6fb73-106">此资源类型继承自 [itemFacet](itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6fb73-107">方法</span><span class="sxs-lookup"><span data-stu-id="6fb73-107">Methods</span></span>

## <a name="methods"></a><span data-ttu-id="6fb73-108">方法</span><span class="sxs-lookup"><span data-stu-id="6fb73-108">Methods</span></span>
|<span data-ttu-id="6fb73-109">方法</span><span class="sxs-lookup"><span data-stu-id="6fb73-109">Method</span></span>|<span data-ttu-id="6fb73-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="6fb73-110">Return type</span></span>|<span data-ttu-id="6fb73-111">说明</span><span class="sxs-lookup"><span data-stu-id="6fb73-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6fb73-112">列表位置</span><span class="sxs-lookup"><span data-stu-id="6fb73-112">List positions</span></span>](../api/profile-list-positions.md)|<span data-ttu-id="6fb73-113">[workPosition](../resources/workposition.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fb73-113">[workPosition](../resources/workposition.md) collection</span></span>|<span data-ttu-id="6fb73-114">从 "位置" 导航属性中获取 workPosition 资源。</span><span class="sxs-lookup"><span data-stu-id="6fb73-114">Get the workPosition resources from the positions navigation property.</span></span>|
|[<span data-ttu-id="6fb73-115">创建 workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-115">Create workPosition</span></span>](../api/profile-post-positions.md)|[<span data-ttu-id="6fb73-116">workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-116">workPosition</span></span>](../resources/workposition.md)|<span data-ttu-id="6fb73-117">创建新的 workPosition 对象。</span><span class="sxs-lookup"><span data-stu-id="6fb73-117">Create a new workPosition object.</span></span>|
|[<span data-ttu-id="6fb73-118">获取 workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-118">Get workPosition</span></span>](../api/workposition-get.md)|[<span data-ttu-id="6fb73-119">workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-119">workPosition</span></span>](../resources/workposition.md)|<span data-ttu-id="6fb73-120">读取 [workPosition](../resources/workposition.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6fb73-120">Read the properties and relationships of a [workPosition](../resources/workposition.md) object.</span></span>|
|[<span data-ttu-id="6fb73-121">更新 workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-121">Update workPosition</span></span>](../api/workposition-update.md)|[<span data-ttu-id="6fb73-122">workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-122">workPosition</span></span>](../resources/workposition.md)|<span data-ttu-id="6fb73-123">更新 [workPosition](../resources/workposition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6fb73-123">Update the properties of a [workPosition](../resources/workposition.md) object.</span></span>|
|[<span data-ttu-id="6fb73-124">删除 workPosition</span><span class="sxs-lookup"><span data-stu-id="6fb73-124">Delete workPosition</span></span>](../api/workposition-delete.md)|<span data-ttu-id="6fb73-125">无</span><span class="sxs-lookup"><span data-stu-id="6fb73-125">None</span></span>|<span data-ttu-id="6fb73-126">删除一个 [workPosition](../resources/workposition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fb73-126">Deletes a [workPosition](../resources/workposition.md) object.</span></span>|


## <a name="properties"></a><span data-ttu-id="6fb73-127">属性</span><span class="sxs-lookup"><span data-stu-id="6fb73-127">Properties</span></span>
|<span data-ttu-id="6fb73-128">属性</span><span class="sxs-lookup"><span data-stu-id="6fb73-128">Property</span></span>|<span data-ttu-id="6fb73-129">类型</span><span class="sxs-lookup"><span data-stu-id="6fb73-129">Type</span></span>|<span data-ttu-id="6fb73-130">说明</span><span class="sxs-lookup"><span data-stu-id="6fb73-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb73-131">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="6fb73-131">allowedAudiences</span></span>|<span data-ttu-id="6fb73-132">String</span><span class="sxs-lookup"><span data-stu-id="6fb73-132">String</span></span>|<span data-ttu-id="6fb73-133">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="6fb73-133">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="6fb73-134">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-134">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="6fb73-135">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6fb73-135">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6fb73-136">categories</span><span class="sxs-lookup"><span data-stu-id="6fb73-136">categories</span></span>|<span data-ttu-id="6fb73-137">String collection</span><span class="sxs-lookup"><span data-stu-id="6fb73-137">String collection</span></span>|<span data-ttu-id="6fb73-138">用户已与此位置关联的类别。</span><span class="sxs-lookup"><span data-stu-id="6fb73-138">Categories that the user has associated with this position.</span></span>|
|<span data-ttu-id="6fb73-139">征求</span><span class="sxs-lookup"><span data-stu-id="6fb73-139">colleagues</span></span>|<span data-ttu-id="6fb73-140">[relatedPerson](../resources/relatedperson.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6fb73-140">[relatedPerson](../resources/relatedperson.md) collection</span></span>|<span data-ttu-id="6fb73-141">与此职位相关联的同事。</span><span class="sxs-lookup"><span data-stu-id="6fb73-141">Colleagues that are associated with this position.</span></span>|
|<span data-ttu-id="6fb73-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="6fb73-142">createdBy</span></span>|[<span data-ttu-id="6fb73-143">identitySet</span><span class="sxs-lookup"><span data-stu-id="6fb73-143">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="6fb73-144">提供创建实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="6fb73-144">Provides the identifier of the user and/or application that created the entity.</span></span> <span data-ttu-id="6fb73-145">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-145">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6fb73-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb73-146">createdDateTime</span></span>|<span data-ttu-id="6fb73-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb73-147">DateTimeOffset</span></span>|<span data-ttu-id="6fb73-148">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="6fb73-148">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="6fb73-149">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-149">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6fb73-150">介绍</span><span class="sxs-lookup"><span data-stu-id="6fb73-150">detail</span></span>|[<span data-ttu-id="6fb73-151">positionDetail</span><span class="sxs-lookup"><span data-stu-id="6fb73-151">positionDetail</span></span>](../resources/positiondetail.md)|<span data-ttu-id="6fb73-152">包含有关职位的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fb73-152">Contains detailed information about the position.</span></span> |
|<span data-ttu-id="6fb73-153">id</span><span class="sxs-lookup"><span data-stu-id="6fb73-153">id</span></span>|<span data-ttu-id="6fb73-154">String</span><span class="sxs-lookup"><span data-stu-id="6fb73-154">String</span></span>|<span data-ttu-id="6fb73-155">用于单独寻址实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="6fb73-155">Identifier used for individually addressing the entity.</span></span> <span data-ttu-id="6fb73-156">继承自 [entity](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="6fb73-156">Inherited from [entity](../resources/entity.md)</span></span>|
|<span data-ttu-id="6fb73-157">推导</span><span class="sxs-lookup"><span data-stu-id="6fb73-157">inference</span></span>|[<span data-ttu-id="6fb73-158">inferenceData</span><span class="sxs-lookup"><span data-stu-id="6fb73-158">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="6fb73-159">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fb73-159">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="6fb73-160">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-160">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6fb73-161">isCurrent</span><span class="sxs-lookup"><span data-stu-id="6fb73-161">isCurrent</span></span>|<span data-ttu-id="6fb73-162">布尔值</span><span class="sxs-lookup"><span data-stu-id="6fb73-162">Boolean</span></span>|<span data-ttu-id="6fb73-163">指示位置是否是最新的。</span><span class="sxs-lookup"><span data-stu-id="6fb73-163">Denotes whether or not the position is current.</span></span>|
|<span data-ttu-id="6fb73-164">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="6fb73-164">lastModifiedBy</span></span>|[<span data-ttu-id="6fb73-165">identitySet</span><span class="sxs-lookup"><span data-stu-id="6fb73-165">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="6fb73-166">提供上次修改实体的用户和/或应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="6fb73-166">Provides the identifier of the user and/or application that last modified the entity.</span></span> <span data-ttu-id="6fb73-167">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-167">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6fb73-168">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6fb73-168">lastModifiedDateTime</span></span>|<span data-ttu-id="6fb73-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6fb73-169">DateTimeOffset</span></span>|<span data-ttu-id="6fb73-170">为创建实体时提供 dateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="6fb73-170">Provides the dateTimeOffset for when the entity was created.</span></span> <span data-ttu-id="6fb73-171">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-171">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="6fb73-172">manager</span><span class="sxs-lookup"><span data-stu-id="6fb73-172">manager</span></span>|[<span data-ttu-id="6fb73-173">relatedPerson</span><span class="sxs-lookup"><span data-stu-id="6fb73-173">relatedPerson</span></span>](../resources/relatedperson.md)|<span data-ttu-id="6fb73-174">包含用户在此位置的经理的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6fb73-174">Contains detail of the user's manager in this position.</span></span>|
|<span data-ttu-id="6fb73-175">source</span><span class="sxs-lookup"><span data-stu-id="6fb73-175">source</span></span>|[<span data-ttu-id="6fb73-176">personDataSource</span><span class="sxs-lookup"><span data-stu-id="6fb73-176">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="6fb73-177">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="6fb73-177">Where the values originated if synced from another service.</span></span> <span data-ttu-id="6fb73-178">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb73-178">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="6fb73-179">关系</span><span class="sxs-lookup"><span data-stu-id="6fb73-179">Relationships</span></span>

<span data-ttu-id="6fb73-180">无。</span><span class="sxs-lookup"><span data-stu-id="6fb73-180">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6fb73-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6fb73-181">JSON representation</span></span>
<span data-ttu-id="6fb73-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fb73-182">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workPosition",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workPosition",
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
  "categories": [
    "String"
  ],
  "detail": {
    "@odata.type": "microsoft.graph.positionDetail"
  },
  "manager": {
    "@odata.type": "microsoft.graph.relatedPerson"
  },
  "colleagues": [
    {
      "@odata.type": "microsoft.graph.relatedPerson"
    }
  ],
  "isCurrent": "Boolean"
}
```